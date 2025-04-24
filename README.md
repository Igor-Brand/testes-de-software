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

## 2. Níveis e Tipos de Teste

### 1. Qual a diferença entre os testes de unidade, integração, sistema e aceitação? Dê um exemplo prático de cada.

- **Teste de Unidade**
  - **Definição:** Testa componentes isoladamente.
  - **Responsável:** Desenvolvedor.
  - **Exemplo:** Verificar se a função `calcularDesconto()` retorna o valor correto com diferentes entradas.

- **Teste de Integração**
  - **Definição:** Testa a comunicação entre componentes.
  - **Exemplo:** Verificar se o módulo de login interage corretamente com o banco de dados de usuários.

- **Teste de Sistema**
  - **Definição:** Avalia o comportamento do sistema completo conforme os requisitos.
  - **Exemplo:** Testar o processo completo de compra em um site de e-commerce (login → adicionar produto → pagamento).

- **Teste de Aceitação**
  - **Definição:** Verifica se o sistema atende às necessidades do usuário final.
  - **Exemplo:** O cliente testa o sistema de agendamento de consultas para validar que ele atende às regras de negócio antes da entrega final.

---

### 2. O que diferencia um teste funcional de um teste não funcional?

- **Teste Funcional**
  - Avalia *o que* o sistema faz.
  - Exemplo: Verificar se o botão "Enviar" de um formulário envia os dados corretamente.

- **Teste Não Funcional**
  - Avalia *como* o sistema se comporta.
  - Exemplo: Medir se o sistema responde em menos de 2 segundos com 100 usuários simultâneos.

---

### 3. O que são testes de regressão e por que eles são importantes?

- **Definição:** Testes realizados após modificações no sistema para garantir que funcionalidades existentes não foram quebradas.
- **Importância:** Mantêm a estabilidade do sistema após correções de bugs, atualizações ou adição de novas funcionalidades.

---

### 4. Quando é apropriado aplicar testes exploratórios em um projeto?

- Quando há poucas ou nenhuma especificação formal.
- Quando há pouco tempo para testar.
- Para complementar testes formais.
- **Importante:** Mais eficaz com testadores experientes, criativos e com conhecimento do domínio.
- **Característica:** O testador aprende, projeta e executa os testes ao mesmo tempo.

---

### 5. Explique a relação entre testes automatizados e testes manuais. Quais são as vantagens e desvantagens de cada abordagem?

- **Teste Manual**
  - **Vantagens:**
    - Ideal para testes exploratórios, usabilidade e UI.
    - Requer pouco tempo inicial para começar.
  - **Desvantagens:**
    - Mais lento.
    - Sujeito a erros humanos.
    - Pouco reutilizável.

- **Teste Automatizado**
  - **Vantagens:**
    - Execução rápida e repetível.
    - Boa cobertura de testes.
    - Ideal para testes de regressão e grandes volumes.
  - **Desvantagens:**
    - Custo inicial elevado.
    - Exige manutenção constante.
    - Nem sempre adequado para testes criativos ou subjetivos.

## 3. Técnicas de Teste

### 1. O que são técnicas de caixa preta e quais exemplos você conhece?

- **Definição:** Técnicas que se concentram no comportamento externo do sistema, sem considerar a estrutura interna do código.
- **Objetivo:** Verificar se o sistema se comporta conforme as especificações.
- **Exemplos:**
  - Particionamento de Equivalência (EP)
  - Análise de Valor Limite (BVA)
  - Teste de Tabela de Decisão
  - Teste de Transição de Estado
  - Teste de Caso de Uso

---

### 2. O que é particionamento de equivalência e como essa técnica ajuda no design de casos de teste?

- **Definição:** Técnica que divide os dados de entrada em classes de equivalência, onde cada classe representa um comportamento semelhante.
- **Objetivo:** Reduzir o número de testes cobrindo todos os cenários relevantes.
- **Exemplo:** Para uma entrada válida entre 1 e 100:
  - Classe válida: 50
  - Classes inválidas: -5, 150

---

### 3. O que é a complexidade ciclomática e como ela é usada para definir o número mínimo de testes?

- **Definição:** Métrica quantitativa que mede a complexidade de um programa, baseada no número de caminhos lineares independentes.
- **Fórmula:** `M = E - N + 2P`
  - *E:* número de arestas no grafo
  - *N:* número de nós
  - *P:* número de componentes conectados
- **Uso:** Ajuda a definir o número mínimo de casos de teste para garantir que cada caminho independente seja testado ao menos uma vez.

---

### 4. Descreva a diferença entre testes de caixa branca e caixa preta com exemplos.

- **Caixa Preta**
  - **Definição:** Testa o comportamento do sistema sem conhecimento interno.
  - **Exemplo:** Testar se uma calculadora retorna o resultado correto ao somar 2 + 2.
- **Caixa Branca**
  - **Definição:** Testa a estrutura interna do código, incluindo fluxos de decisão.
  - **Exemplo:** Verificar se todos os ramos de uma instrução `if-else` são executados.

---

### 5. O que são testes baseados em experiência e quando eles devem ser utilizados?

- **Definição:** Técnica que usa o conhecimento, intuição e histórico do testador para encontrar defeitos.
- **Exemplos:**
  - Teste Exploratório
  - Teste Baseado em Checklists
  - Ataques de Teste (Test Attacks)
- **Quando usar:**
  - Quando há pouca documentação.
  - Em sistemas críticos onde a experiência do testador pode encontrar problemas que testes sistemáticos não encontram.
  - Para descobrir problemas ocultos ou inesperados.

---
## 4. Processo de Teste

### 1. Quais são as etapas típicas de um processo de teste completo, desde o planejamento até o encerramento?

Um processo de teste típico é composto pelas seguintes etapas:

1. **Planejamento de Teste:** Definição do escopo, objetivos, abordagem e cronograma.
2. **Análise de Teste:** Análise dos requisitos para identificar condições de teste.
3. **Projeto de Teste:** Criação dos casos de teste, critérios de entrada e saída.
4. **Implementação e Execução:** Execução dos casos de teste, registro dos resultados.
5. **Avaliação de Critérios de Saída:** Verificação se os critérios de término foram atendidos.
6. **Encerramento de Teste:** Finalização da documentação, arquivamento e lições aprendidas.

---

### 2. O que é um plano de testes e quais informações ele deve conter?

- **Definição:** Documento que descreve a estratégia, objetivos, cronograma e recursos necessários para o processo de teste.
- **Deve conter:**
  - Escopo e objetivos
  - Itens a serem testados
  - Estratégia de testes
  - Critérios de entrada e saída
  - Cronograma
  - Recursos (ferramentas, pessoas, ambientes)
  - Riscos e contingências
  - Responsabilidades

---

### 3. Como funciona o ambiente de testes e por que ele deve ser isolado?

- **Definição:** Conjunto de hardware, software, redes e ferramentas necessárias para realizar os testes.
- **Deve ser isolado para:**
  - Evitar interferência com sistemas de produção
  - Garantir consistência e repetibilidade dos testes
  - Permitir controle total do ambiente (dados, configurações, versões)
- **Pode incluir:** bancos de dados específicos, servidores dedicados, ferramentas de automação, etc.

---

### 4. Qual o papel do engenheiro de testes dentro de um projeto ágil?

- **Responsabilidades:**
  - Colaborar com desenvolvedores e POs para definir critérios de aceitação
  - Automatizar testes sempre que possível
  - Garantir a qualidade contínua com testes frequentes
  - Participar de reuniões de planejamento e retrospectiva
  - Atuar como facilitador de qualidade em todo o ciclo de desenvolvimento
- **Papel ativo:** o engenheiro de testes está envolvido desde o início e trabalha de forma contínua com a equipe.

---

### 5. Quais documentos de teste são definidos pela norma IEEE 829-1998?

A norma IEEE 829-1998 define os seguintes documentos de teste:

1. **Plano de Testes (Test Plan)**
2. **Especificação de Caso de Teste (Test Case Specification)**
3. **Especificação de Procedimento de Teste (Test Procedure Specification)**
4. **Especificação de Item de Teste (Test Item Transmittal Report)**
5. **Registro de Teste (Test Log)**
6. **Relatório de Incidentes (Test Incident Report)**
7. **Relatório de Sumário de Teste (Test Summary Report)**

Cada documento tem um propósito específico no ciclo de vida do teste, promovendo padronização e rastreabilidade.

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
