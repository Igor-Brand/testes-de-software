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
## 5. Engenharia de Requisitos

### 1. O que são requisitos funcionais e não funcionais? Dê exemplos reais.

- **Requisitos Funcionais:** descrevem *o que o sistema deve fazer*. Exemplo:
  - "O sistema deve permitir que o usuário realize login com e-mail e senha."
  - "O sistema deve calcular o valor total de uma compra com base nos itens do carrinho."

- **Requisitos Não Funcionais:** descrevem *como o sistema deve se comportar*. Exemplo:
  - "A aplicação deve carregar a página inicial em no máximo 3 segundos."
  - "O sistema deve estar disponível 24 horas por dia, 7 dias por semana."

---

### 2. O que são regras de negócio e como elas impactam os testes?

- **Definição:** São políticas, restrições ou condições específicas do domínio do negócio que afetam como o sistema deve se comportar.
- **Exemplo:** "Clientes com mais de 5 compras no mês recebem 10% de desconto."
- **Impacto nos testes:**
  - Os testes devem verificar se as regras estão corretamente implementadas.
  - Casos de teste devem considerar todas as variações possíveis das regras.
  - A complexidade das regras pode demandar testes mais elaborados e específicos.

---

### 3. Quais técnicas podem ser utilizadas para o levantamento de requisitos? Cite ao menos três.

1. **Entrevistas:** Conversas estruturadas com stakeholders para entender as necessidades.
2. **Workshops:** Sessões colaborativas com clientes e equipe técnica.
3. **Observação direta:** Análise de como os usuários interagem com sistemas atuais.
4. **Questionários:** Coleta de informações de um grupo maior de usuários.
5. **Protótipos:** Criação de maquetes para validação rápida de ideias.

---

### 4. Por que é importante registrar toda comunicação entre analista, cliente e equipe de desenvolvimento?

- Para garantir **clareza e rastreabilidade** das decisões.
- Evita **mal-entendidos** e **requisitos ambíguos**.
- Facilita o **gerenciamento de mudanças**.
- Serve como base para **validação e testes** futuros.
- Ajuda na documentação e histórico do projeto.

---

### 5. Qual a relação entre engenharia de requisitos e a definição de critérios de aceitação nos testes?

- Os **critérios de aceitação** são definidos com base nos **requisitos funcionais e regras de negócio**.
- Uma boa engenharia de requisitos fornece **informações claras e completas** que ajudam a criar critérios mensuráveis.
- Permite que os testes sejam objetivos e verificáveis, garantindo que o sistema atenda às expectativas do cliente.
- Serve como base para **testes de aceitação**, fundamentais no modelo ágil.

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

---

## 6. Testes Ágeis e Qualidade

### 1. O que significa o termo “Test-Driven Development (TDD)” e como ele funciona?

- **Test-Driven Development (TDD)** é uma técnica de desenvolvimento onde os testes são escritos antes mesmo do código de produção.
- **Como funciona:**
  1. **Escreve-se um teste:** O desenvolvedor cria um teste simples que falha, pois o código ainda não foi implementado.
  2. **Escreve-se o código:** O desenvolvedor escreve o código mínimo necessário para fazer o teste passar.
  3. **Refatora:** O código é melhorado, se necessário, mantendo os testes passando.
  4. **Repete:** O ciclo é repetido para cada nova funcionalidade.

TDD promove **alta cobertura de testes**, **código mais limpo** e **feedback rápido** sobre o comportamento do sistema.

---

### 2. Explique as diferenças entre verificação e validação no contexto dos testes.

- **Verificação:** É o processo de garantir que o produto foi construído corretamente, ou seja, que **atende aos requisitos especificados**. A verificação responde à pergunta "Estamos construindo o produto certo?"
  - **Exemplo:** Revisão de código, análise de requisitos, inspeções.
  
- **Validação:** É o processo de garantir que o produto correto foi construído, ou seja, que **atende às necessidades do cliente**. A validação responde à pergunta "Estamos construindo o produto da maneira certa?"
  - **Exemplo:** Testes de aceitação, testes funcionais.

---

### 3. O que são critérios de aceitação e qual sua importância nos testes ágeis?

- **Critérios de aceitação** são condições específicas que um produto ou funcionalidade deve cumprir para ser considerado pronto e aceito pelo cliente.
  - São definidos em colaboração com o cliente ou stakeholder e descrevem claramente **o que é considerado uma entrega bem-sucedida**.
  
- **Importância nos testes ágeis:**
  - **Garantem alinhamento** com as expectativas do cliente.
  - Servem como base para **testes de aceitação**.
  - Facilitam a **comunicação contínua** entre a equipe de desenvolvimento e os stakeholders.
  - Permitem uma **avaliação objetiva** de quando uma funcionalidade está pronta.

---

### 4. Quais são as fases de execução de testes em uma abordagem ágil?

1. **Planejamento do Sprint:** Definição dos requisitos e critérios de aceitação.
2. **Desenvolvimento e Testes:** A equipe de desenvolvimento cria o código, enquanto os testes são executados ao longo do processo.
3. **Testes de Aceitação:** Testes baseados nos critérios de aceitação definidos previamente, realizados pelos desenvolvedores ou testers.
4. **Feedback Contínuo:** O feedback é fornecido rapidamente após a execução dos testes, permitindo ajustes imediatos no desenvolvimento.
5. **Revisão do Sprint:** Análise dos resultados dos testes, validação da entrega e identificação de melhorias.

---

### 5. Como a adoção de ferramentas de testes automatizados pode contribuir para a qualidade do produto?

- **Contribuições para a qualidade do produto:**
  1. **Redução de erros humanos:** As ferramentas automatizadas reduzem a chance de falhas causadas por erros manuais.
  2. **Execução contínua:** Testes podem ser executados rapidamente e com frequência, proporcionando **feedback imediato**.
  3. **Cobertura de testes mais ampla:** Com a automação, é possível cobrir uma **maior quantidade de cenários** e casos de teste.
  4. **Economia de tempo e custo:** Testes repetitivos são mais rápidos e menos dispendiosos quando automatizados.
  5. **Facilidade de manutenção:** Os testes podem ser **atualizados e reutilizados** de maneira simples conforme o sistema evolui.
  
A automação melhora **a eficiência** dos testes e **a confiabilidade** do produto.

---
