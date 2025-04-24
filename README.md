# testes-de-software
Repositório para matéria de software
---
### **1. Fundamentos e Conceitos Gerais*

1. **Teste de software** é o processo de avaliar e verificar se um software atende aos requisitos e está livre de defeitos. É essencial para garantir qualidade, evitar falhas em produção e aumentar a confiabilidade.
    
2. **Erro**: ato humano que gera um problema;  
    **Defeito (bug)**: imperfeição no código causada por um erro;  
    **Falha**: quando o defeito é executado e o software não se comporta como esperado.
    
3. **Sete princípios do teste (ISTQB)**:
    
    - Testes mostram a presença de defeitos
        
    - Testes exaustivos são impossíveis
        
    - Testes antecipados economizam tempo e dinheiro
        
    - Agrupamento de defeitos
        
    - O paradoxo do pesticida
        
    - Testes dependem do contexto
        
    - A ilusão de ausência de erros
        
4. Quanto **mais defeitos encontrados** durante os testes, **mais confiável tende a ser o software**, desde que os defeitos sejam corrigidos. A confiabilidade é a capacidade de operar sem falhas.
    
5. A **ISO/IEC 9126** define **atributos de qualidade** como: funcionalidade, confiabilidade, usabilidade, eficiência, manutenibilidade e portabilidade.

---
### **2. Níveis e Tipos de Teste**

1. - **Unidade**: testam funções/métodos isolados (ex: testar a função de login);
        
    - **Integração**: testam módulos em conjunto (ex: integração entre frontend e backend);
        
    - **Sistema**: testam o sistema como um todo (ex: verificar fluxo completo de compra);
        
    - **Aceitação**: validados por usuários/clientes (ex: cliente verifica se o sistema atende aos requisitos).
        
2. - **Funcional**: verifica _o que_ o sistema faz (ex: login, cadastro);
        
    - **Não funcional**: verifica _como_ o sistema se comporta (ex: desempenho, segurança).
        
3. **Testes de regressão** garantem que novas alterações não quebrem funcionalidades existentes. São importantes após correções ou adição de novas funcionalidades.
    
4. Usam-se **testes exploratórios** quando não há muita documentação ou quando se quer descobrir erros através da criatividade e experiência do testador.
    
5. - **Automatizados**: rápidos e repetíveis (ex: testes com Selenium).  
        _Vantagens_: consistência, velocidade.  
        _Desvantagens_: custo de manutenção.
        
    - **Manuais**: feitos por humanos.  
        _Vantagens_: flexibilidade, testes subjetivos.  
        _Desvantagens_: mais lentos e suscetíveis a erros humanos.

---

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
    
3. O **ambiente de testes** simula o ambiente de produção e deve ser **isolado** para garantir resultados controlados e não impactar sistemas reais.
    
4. Em **projetos ágeis**, o engenheiro de testes atua de forma contínua, colaborando com desenvolvedores e POs, garantindo que requisitos estejam claros e testáveis desde o início.
    
5. A **IEEE 829-1998** define documentos como: plano de teste, casos de teste, relatório de testes, logs de execução, relatório de incidentes, entre outros.
