# testes-de-software
Repositório para matéria de software
---
# **1. Fundamentos e Conceitos Gerais*
# Teste de Software

## 1. O que é teste de software e por que ele é considerado essencial no desenvolvimento de sistemas?

O teste de software é uma forma de **controle de qualidade** que envolve a avaliação de produtos de trabalho de software por meio de:

- Exame manual (revisões)
- Ferramentas (análise estática)
- Execução do software (teste dinâmico)

### Objetivos do teste:
- Melhoria da qualidade
- Detecção de defeitos
- Avaliação de características como:
  - Legibilidade
  - Integridade
  - Correção
  - Testabilidade
  - Consistência

### Importância:
- Garante que o sistema funcione conforme esperado pelos stakeholders
- Ajuda a atingir os objetivos dentro do escopo, tempo, qualidade e orçamento
- Oferece uma representação indireta dos usuários no desenvolvimento
- Pode ser necessário para requisitos contratuais, legais ou normas regulatórias

---

## 2. Qual a diferença entre erro, defeito e falha no contexto de teste de software?

- **Erro**: Ação humana que produz um resultado incorreto.
- **Defeito (bug)**: Resultado de um erro que pode, se executado, causar uma falha.
- **Falha**: Evento no qual um componente ou sistema não executa sua função dentro das tolerâncias especificadas.
- **Causa-raiz**: Motivo fundamental para a ocorrência de um problema, levando a um erro.

---

## 3. Quais são os sete princípios fundamentais do teste de software de acordo com o ISTQB?

1. **O teste mostra a presença, não a ausência de defeitos**  
   Testes indicam que há defeitos, mas não garantem que não existam outros.

2. **Testes exaustivos são impossíveis**  
   Exceto em casos triviais, é inviável testar todas as combinações de entradas.

3. **Testes devem começar cedo (early testing)**  
   Quanto mais cedo no ciclo de vida, melhor. A abordagem "shift-left" é recomendada.

4. **Agrupamento (clustering) de defeitos**  
   Poucos módulos tendem a conter a maioria dos defeitos.

5. **Paradoxo do pesticida**  
   Testes repetidos perdem eficácia; é necessário revisar e criar novos testes.

6. **Os testes dependem do contexto**  
   A abordagem deve se adaptar ao tipo de sistema ou produto.

7. **Falácia da ausência de defeitos**  
   Um software sem defeitos ainda pode não atender às necessidades dos usuários ou aos objetivos do negócio.

---

## 4. Como o conceito de confiabilidade do software se relaciona com a quantidade de defeitos encontrados?

- A **confiabilidade** é uma característica de qualidade **não funcional**.
- **Testes não funcionais** avaliam atributos como confiabilidade.
- Encontrar e corrigir defeitos contribui para **melhorar a confiabilidade** do software.
- **Métricas de defeitos** (número de defeitos encontrados, densidade de defeitos, etc.) são usadas para rastrear a qualidade do produto.
- Conclusão: embora não haja uma relação quantitativa direta explícita, **menos defeitos = maior confiabilidade**.

---

## 5. O que a norma ISO/IEC 9126 estabelece sobre os atributos de qualidade de software?

- A norma **ISO/IEC 9126** não é mencionada diretamente nos materiais fornecidos.
- No entanto, os materiais referem a norma **ISO 25010**, que atualiza e complementa a 9126.
- Características de qualidade citadas:
  - Adequação funcional
  - Eficiência de performance
  - Compatibilidade
  - Usabilidade
  - Confiabilidade
  - Segurança
  - Manutenibilidade
  - Portabilidade

Essas características são avaliadas principalmente por **testes não funcionais**.

### **3. Técnicas de Teste**

1. - **Caixa preta**: foco nas entradas/saídas (ex: testes funcionais, particionamento de equivalência).
        
    - Exemplos: particionamento, análise de valores-limite.
        
2. **Particionamento de equivalência** divide dados de entrada em classes onde o comportamento do sistema é o mesmo, reduzindo número de testes.
    
3. **Complexidade ciclomática** mede o número de caminhos independentes num código. Ajuda a definir o número mínimo de testes necessários para cobrir o fluxo lógico.
    
4. - **Caixa branca**: testa o código internamente (ex: cobertura de branches);
        
    - **Caixa preta**: testa as funcionalidades sem ver o código (ex: input/output esperados).
        
5. **Testes baseados em experiência** dependem da intuição e conhecimento prévio do testador. São úteis em sistemas novos ou mal documentados.

---
### **4. Processo de Teste**

1. - Planejamento
        
    - Análise e design dos testes
        
    - Implementação
        
    - Execução
        
    - Avaliação dos critérios de saída
        
    - Encerramento dos testes
        
2. **Plano de testes**: define escopo, objetivos, recursos, cronograma, critérios de entrada/saída, riscos e estratégias de teste.

---


### **6. Testes Ágeis e Qualidade**

1. **TDD (Test-Driven Development)**: escreve-se o teste antes do código. O ciclo é: escrever teste → escrever código → refatorar → repetir.
    
2. - **Verificação**: verifica se o sistema foi construído corretamente;
        
    - **Validação**: verifica se o sistema certo foi construído (atende ao que o cliente quer).
        
3. **Critérios de aceitação** são condições que definem quando uma funcionalidade está pronta. Servem como base para testes em ambientes ágeis.
    
4. - Planejamento de testes
        
    - Preparação do ambiente
        
    - Execução contínua (a cada sprint)
        
    - Feedback e melhoria contínua
        
5. **Automação** acelera testes de regressão, aumenta cobertura, reduz erros humanos e garante entregas mais rápidas e seguras.
    
4. O **ambiente de testes** simula o ambiente de produção e deve ser **isolado** para garantir resultados controlados e não impactar sistemas reais.
    
5. Em **projetos ágeis**, o engenheiro de testes atua de forma contínua, colaborando com desenvolvedores e POs, garantindo que requisitos estejam claros e testáveis desde o início.
    
6. A **IEEE 829-1998** define documentos como: plano de teste, casos de teste, relatório de testes, logs de execução, relatório de incidentes, entre outros.
