# Projeto da Disciplina de Desenvolvimento Web Mobile

## Frameworks

Um framework é um conjunto de conceitos usados para resolver um problema em um domínio específico. Conceitualmente, um framework não é um software executável, mas sim um conjunto de diretrizes para um domínio.

### Frameworks de Software

Um framework de software compreende um conjunto de classes implementadas em uma linguagem de programação específica usadas para auxiliar no desenvolvimento de software.

## Frameworks Introdutórios para Desenvolvimento Web

### Bootstrap

- O mais popular framework HTML, CSS e JavaScript para desenvolvimento de projetos responsivos.
- Originalmente desenvolvido para o Twitter, posteriormente se tornou uma das estruturas front-end de código aberto mais populares do mundo.

### jQuery

- Biblioteca JavaScript cross-browser desenvolvida para simplificar os scripts client-side.

## Capítulo II - Padrões Arquiteturais

Padrões arquiteturais definem a estrutura, interações e organização dos componentes do software, facilitando a comunicação entre desenvolvedores e garantindo escalabilidade, manutenção e reutilização do código.

### Padrões Existentes

- **Monolítico**
- **Microserviços**
- **Modelo-Visão-Controlador (MVC)**

### Padrão Arquitetural Monolítico

- **Vantagens:**
  - Facilidade inicial para criar uma solução única, interligando todas as funcionalidades do sistema.
- **Problemas:**
  - Escalabilidade limitada
  - Dificuldade de agregação de tecnologias
  - Demora no aculturamento para novos integrantes
  - Aumento de complexidade e tamanho ao longo do tempo
  - Falta de flexibilidade
  - Dificuldade para implementar alterações em produção

### Padrão Arquitetural Microserviços

- **Características:**
  - Separação dos elementos de funcionalidade em serviços separados e autônomos que se comunicam por meio de APIs.
  - Cada funcionalidade é separada em serviços com escopo bem definido que podem complementar outras funcionalidades.
- **Principal Dificuldade:**
  - Necessidade de desenvolvedores qualificados

### Padrão Arquitetural Modelo-Visão-Controlador (MVC)

- **Descrição:**
  - O padrão MVC separa a **representação** da **informação** da **interação** do usuário com o sistema.
  - Alterações feitas no layout não afetam a manipulação de dados, permitindo reorganizações sem alterar o layout.
  - Proporciona separação das tarefas de **acesso aos dados**, **lógica de negócios**, **apresentação** e **interação** com o usuário, introduzindo o componente **Controlador**.

- **Componentes:**
  - **Modelo (Model):**
    - Consiste nos dados da aplicação, regras de negócios, lógica e funções.
  - **Visão (View):**
    - Representação dos dados, como tabelas ou diagramas. Pode ter várias representações para o mesmo dado.
  - **Controlador (Controller):**
    - Media a entrada, convertendo-a em comandos para o modelo ou visão. A ideia central do MVC é a reusabilidade de código e a separação de conceitos.

- **Fluxograma MVC:**
  1. O usuário envia um pedido de URL.
  2. O controlador pede dados ao modelo.
  3. O modelo devolve os dados pedidos.
  4. O controlador seleciona a visão e fornece os dados.
  5. A visão selecionada é devolvida ao controlador.
  6. O controlador devolve a visão como resposta para o navegador.

- **Model-View-Template (MVT):**
  - **Model:** Camada de acesso aos dados, geralmente responsável pelo acesso ao banco de dados.
  - **Template:** Camada de apresentação da informação, que lida com a interface para o usuário.
  - **View:** Camada que implementa a lógica de negócios e interage com o modelo para transportar dados e renderizar um template.

### Mapeamento Objeto-Relacional (ORM)

- Técnica de desenvolvimento utilizada para reduzir a demanda de trabalho em programação orientada a objetos ao utilizar bancos de dados relacionais.
- As tabelas do banco de dados são representadas através de classes e os registros como instâncias das classes correspondentes.
- Simplifica o trabalho com persistência de dados, isolando o código do programa das alterações à organização dos dados nas tabelas.
- Ferramentas gráficas como o ORM Pony (https://ponyorm.org/) podem ser usadas para gerar o código que representa o modelo do banco.

## Capítulo III

### Levantamento de Requisitos

- Propicia que usuários e desenvolvedores tenham a mesma compreensão do problema a ser resolvido.

### Análise

- Construir modelos que determinam o problema para o qual estamos tentando conceber uma solução de software.

### Projeto

- Adaptar o modelo de análise para que possa servir como base para a implementação.

### Codificação (Implementação)

- A codificação do sistema é efetivamente executada.

### Teste

- Consiste na verificação do software.

### Implantação

- Entrada em produção do sistema.

## Desenvolvimento Ágil

- **Agilidade:** Capacidade de responder adequadamente a mudanças (software, equipe, tecnologias).
- Adequado para gerenciamento de requisitos e prioridades instáveis (voláteis).
- Projeto e construção são realizados simultaneamente.
- Análise, projeto, implementação e testes não são tão previsíveis (planejamento).

### Manifesto Ágil

- Declaração de princípios que fundamentam o desenvolvimento ágil de software.

### Metodologias Ágeis

- **Extreme Programming (XP)**
  - Cliente presente: O cliente deve participar ativamente do processo de desenvolvimento.
  - Planejamento: Desenvolvimentos são feitos em iterações (1 ou 2 semanas).
  - Releases curtos: Liberações de pequenas versões funcionais ajudam no processo de aceitação do cliente.

- **Práticas de XP:**
  - **Stand-up meetings:** Reuniões rápidas e em pé, geralmente envolvendo perguntas sobre progresso e impedimentos.
  - **Programação em pares:** Duas pessoas programando juntas em um único computador para melhorar a qualidade do código.
  - **Semana de 40 horas:** Ritmo de trabalho saudável, com 40 horas semanais.
  - **Testes constantes:** Uso do Desenvolvimento Orientado a Testes (TDD).
  - **Refatoração:** Melhoria contínua da programação.
  - **Padronização do código:** Regras para manter a consistência do código.

- **Scrum**
  - Metodologia ágil para gestão e planejamento de projetos, especialmente de pequeno ou médio porte.
  - Funcionalidades são mantidas em uma lista chamada Product Backlog.
  - O Product Backlog é dividido em ciclos chamados sprints (tipicamente quinzenais ou mensais).
  - **Sprint Planning Meeting:** Reunião de planejamento onde o Product Owner prioriza itens do Product Backlog e a equipe seleciona as atividades para o sprint.
  - **Daily Scrum:** Reunião diária para disseminar conhecimento.
  - **Sprint Review Meeting:** Apresentação das funcionalidades implementadas.
  - **Sprint Retrospective:** Reflexão sobre o sprint e planejamento do próximo.

## Django Framework

- Django é um framework web Python de alto nível, livre e open-source que encoraja o desenvolvimento rápido e limpo.
- Utiliza o princípio DRY (Don't Repeat Yourself), permitindo reutilizar código e evitando repetição.
- Utilizado para o desenvolvimento do backend do Instagram.
- Django utiliza uma variante do padrão arquitetural MVC chamada MVT (Model-View-Template).

### Componentes do Django

- **Model:** Camada de acesso a dados, responsável por definir dados, validações e relacionamentos.
- **View:** Camada intermediária que associa modelos a templates e pode conter regras de negócios.
- **Template:** Camada de apresentação que lida com a interface e a forma como os dados são apresentados.

### Principais Características

- **URLs Amigáveis:** Criação de URLs simples e amigáveis.
- **Sistema de Cache:** O framework possui um sistema de cache para melhorar o desempenho.

## Unified Modeling Language (UML)

- A UML é uma linguagem de notação essencial para diversas etapas da criação de um software orientado a objetos, usando elementos gráficos para documentação.

### Diagramas Estruturais

- Modelam aspectos estáticos do software, como métodos, interfaces, serviços, arquiteturas e classes.
  - Exemplos: Diagrama de Classes, Diagrama de Componentes, Diagrama de Implantação, Diagrama de Objetos, Diagrama de Pacotes.

### Diagramas Comportamentais

- Especificam detalhes do comportamento do software e o que deve acontecer no sistema.
  - Exemplos: Diagrama de Caso de Uso, Diagrama de Atividades, Diagrama de Máquina de Estado, Diagrama de Sequência.

## Aula 5

### Métodos HTTP

- **GET:** Solicita a representação de um recurso. Não deve ser usado para disparar ações (ex: remover um usuário).
- **POST:** Envia informações no corpo da requisição para criar um novo recurso.
- **DELETE:** Remove um recurso. Deve retornar o status 204 se o recurso não existir.
- **PUT:** Atualiza um recurso na URI especificada. Pode criar um novo recurso se não existir.

### Status Codes

- **2xx Success:**
  - 200 OK
- **3xx Redirection:**
  - 301 Moved Permanently
  - 302 Found (Temporary Redirect)
  - 304 Not Modified
- **4xx Client error:**
  - 401 unathorized error
  - 403 forbidden
  - 404 not found
  - 405 method not allowed
- **5xx server error:**
  - 502 not implemented
  - 502 bad gateway
  - 503 service unavaliable
  - 504 gatewat timeout

### CLASS BASED VIEWS
- Sçao views (django) com base em classes (python) em funções. Isto signidica que oara domina-las é preciso entender tatno as views em django

## Próxima Aula Fazer tela de login interface