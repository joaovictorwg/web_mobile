Projeto da disciplina de Desenvolvimento Web Mobile

Frameworks

um framework é um conjunto de conceitos usados para resolver um problema de um dominio especifico

um framework, conceitualmente, não se trata de um software executavel, mas sim de dados para um dominio

framework de software compreende de um conjunto de classes implementadas em uma linguagem de progranaçao especifica usadas para auxiliar o desenvolvimento de software

# Frameworks introdutoerios para desenvolvimento web

## bootstrap
- o mais popular framework html, css e js para desenvolvimento de projetos responsivos
- originalmente foi desenvolvido para o twitter. Posteriormente, se tornou uma das estruturas front-end de codigo aberto mais populares do mundo

## JQuery
- Biblioteca javascript cross-browser desenvolvida para simplificar os scripts client-side

# Capitulo II - Padrões Arquiteturais
- Definem a estritira, interações e organização dos componentes do software, facilitando a comunicação entre desenvolvedores e garantindo escalabilidade, manutenção e reutilização do codigo

- ### Padrões existentes
  - Monolitico
  - Microserviços
  - modelo-Visão-Controlador(MVC)
- Aplicação formada por modulos que mesmo agindo separadamente, continuam ligados, transformando o conjunto em um unico sistema.
  
- #### Padrão Arquitetural Monolítico
  - Facilidade (inicialmente) para cirar uma solução unica, interligando todas as funcionalidades do sistema
  - problemas: escalabilidade, agregação de tecnologias, demora no aculturamento para novos integrantes, aumento de complexidade e do tamanho longo do tempo, falta de flexibilidade, dificuldade para colocar alterações em produção
- #### Padrão Arquitetural Microserviçoes
  - Provê a separação dos elementos de funcionalidade, colocados em serviçoes separados, dessa forma, tornando-os totalmente autônomos e totalmente independentes, que se comum=nicam por meio de APIs
  - Cada funcionalidade é separada em serviços de funcionalidade/escopo bem definido que podem ou não complementar outra funcionalidade
  - Principal dificuldade: necessidade de desenvolvedores qualificados
  
- ### Padrão Arquitetural Modelo-Visão-Controlador(MVC)
  - Model-View-Controller é um padrão de arquitetura de software que **separa** a **representação** da **informação** da **interação** do usuário com ele
  - Alterações feitas no layout não afetam a mannipulação de dados, e estes poderão ser reorganizados sem alterar o layout
  - Provê a **separação** das tarefas de a**cesso aos dados** e **logica de negocio**, logica de **apresentaçã**o e de **interação** com o utilizados, introduzindo um componente entre os dois: o **controlador**

  - #### MODELO(MODEL)
    - Consiste nos dados da aplicação, regras de negócios, lógica e funções
  - #### VISÃO(VIEW)
    - Pode ser qualquer saida de representação dos dados, como uma tabela ou um diagrama. É possível ter várias cisões do mesmo dado, cono un grafico de barras para gerenciamento e uma visão tabular para contadores.
  - #### CONTROLADOR(CONTROLLER)
    - Faz e mediação da entrada, convertendo-a em comandos para o modelo ou visão. As ideias centrais por trás do MVC são a reusabilidade de código e a separação de conceitos.
  - #### Fluxograma MVC
    - 1. O usuário envia um pedido de url
    - 2. O controlador pede dados ao modelo
    - 3. O modelo devolve os dados pedidos
    - 4. O controlador seleciona a visão e fornece os dados
    - 5. A visão selecionada é devolvida ao controlador
    - 6. O controlador devolve a visão como resposta para o browser 
  - #### Model View Template (MVT)
    - Model: Representa a camada de acesso aos dados, geralmente é responsável pelo acesso ao banco de dados.
    - Template: camada de apresentação da informação, que lida com a interface para o usuário
    - View: camada usada para implementar a lógica de negócios e interagir com um modelo para transportar dados e renderizar um template.
  
- ### Mapeamento Objeto Relacional - ORM
  - Técnica de desenvolvimento utilizada para reduizir demanda de trabalho em programação orientada a objetos ao se utilizar bancos de dados relacionais
  - As tabelas do banco de dados são representadas através de clasees e os registros de cada tabela são representados como instâncias das classes correspondentes.
  - Com esta tecnica, o progreamador não precisa se preocupar com os comandos em linguagem SQL. Ele irá, usar uma interface de programação simples que faz todo o trabalho de persistência.
  - Não é necessária uma correspondência direta entre as tabelas de dados e as cklasses do progama
  - A relação entre as tabelas onde originam os dados e o objeto que os disponibiliza é configurada pelo programador, isolando o codigo do programa das alterações à organização dos dados nas tabelas do banco de dados.
  - A forma como este mapeamento é configurado depende da ferramenta utilizada. Como exemplo, o progamador que usa hibernate na linguagem Java pode usar arquivos XML, ou o sistema de anotações(annotations) que a linguagem providencia. Em outros casos o mapeamento é feito diretamente no codigo, atreaves da herança de classes especiais como é o caso do ORM do django e do SqlAlchemy na linguagem python
  - **Simplicidade, facilidade e produtividade**
  - Algumas ferramentas gráficas podem ser usadas para gerar o codigo que representa o modelo do banco, como o ORM Pony https://ponyorm.org/ também da linguagem python.
  - A forma como este mapeamento é configurado depende da ferramenta utilizada

