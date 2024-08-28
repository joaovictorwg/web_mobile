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

# Capitulo III
- Levantamento de requisitos: propiciar que usuarios e desenvolvedores tenham a mesma compreensão do problema a ser resolvido
- Análise: construir modelos que determinam qual é o problema apra o qual estamos tentando conceber uma solução de software
- Projeto: estágio no qual o modelo de análise terá de ser adaptado de tal modo que possa servir como base para implementação alvo.
- Codificação (implementação): a codigicação do sistmea é efetivamente executada
- Teste: Consiste na verificação do software. Implantação: entrada em produção do sistema
### Desenvolvimento agil
- Agilidade: capacidade de responder adequadamente á mudanças (software, equipe, tecnologias)
- Adequado para gerenciamento de requisitos e prioridades instaveis (volateis)
- Projeto e construção são realizados simultaneamente
- Analise, projeto, implementação e testes não são tão previsiveis (planejamento)
- O manifesto agil: declaração de principios que fundamentam o desenvolvimento agil de software
- Ex. metodologias ágeis: Extreme programming (XP) e Scrum.
#### Extreme Programming
- CLiente presente: o cliente deve participar ativamente do processo de desenvolvimento, facilitando a comunicação, acompanhando o progesso e sendo informado sobre mudanças
- Planejamento> o desenvolviemnto utilizando o XP é feito em iterações. Uma iteração é um periodo curto de tempo (1 ou 2 semanas) onde a equipe desenvolve um conjunto de funcionalidades
- Releases curtos: As liberações de pequenas versões funcionais do projeto auxiliam muito no processo de aceitação por parte do cliente que ja pode testar uma parte do sistema.
##### Baseada em práticas, como:
- Stand up meeting: São reuniões feitas em pe e de curta duração, geralmente envolvendo as seguintes perguntas: o que você fez no dia anterior? o que vai fazer hoje? existe algum impedimento? Ainda que apareça algum problema, essa reunião não tem propósito de pensar em soluções.
- Programações em pares: programação em pares (duplas) em um único computador. Busca-se sempre evolução da equipe melhorando a qualidade do código fonte.
- Semana de 40 horas: trabalhar com qualidade buscando ter um ritimo de trabalho saudavel, 40 horas por semana, 8 horas por dia
- Testes constantes: utiliza-se o Desenvolvimento Orientado a Testes (test driven development) o conhecimento TDD
- Refaração: processo que permite a melhoria continua da programação. Refatorar melhora clareza, leitura do codigo, e facilita manutenção
- Padronização do código: como todo mundo trabalha no desenvolvimento do mesmo software, a equipe de desenvolvimento precisa estabelecer regras para programar e todos devem seguir essas regras, assim parecerá que o codigo fonte foi digitado pela mesma pessoa
### Scrum
- metodologia agil para gestão e planejamento de projeto de software, especialmente de pequeno ou medio porte. Projetos de grande complexidade exigem processos mais complexos (RUP)
- As funcionalidades a serem implementadas em um projeto são mantidas em uma lista que é conhecida como product backlog
- no scrum, o escopo do projeto (product backlog) é dividido em ciclos (tipicamente quinzenais ou mensais) chamados de sprints
- no inicio de cada sprint, faz-se um sprint planning meeting, ou seja, uma reuniçao de planejamento na qual o Product Owner prioriza os itens do Product Backlog Item e a equipe seleciona as atividades que ela sera capaz de implkementar durante o sprint que se inicia 
- As tarefas alocadas em um sprint são transferidas do product Backlog para o sprint backlog. A cada dia de uma sprint a equipe faz um breve reunião(normalmente pela mannha) chamada daily scrum. O objetivo é disseminar conhecimento
- Ao final de um sprint, a equipe apresenta as funcionalidades implemnetadas em uma sprint review meeting. Finalment, faz-se uma sprint Retrospective e a equipe parte para o planejamento do proximo sprint, Assim reinicia-se o ciclo

## Django Framework
- Django é um web framework python de alto nivel, livre e opensource que encoraja o desenvolvomento rapido e limpo e o design programatico
- construido por desenvolvedores experientes, toma conta de muitos dos aborrecimentos do desenvolvimento web, assim, o desenvolvedor pode manter o foco na implementação da aplicação
- O django utiliza o principio dru (dont repeat tourself), que permite ao desenvolvedor aproveitas ao maximo o codigo ja feito, evitando repetição
- utilizado para o desenvolvimento do backend do aplicativo mobile do instagram
- Django utiliza uma variante (MVT) do padrão arquitetural mvc
- Model: camada de acesso a dados. Contem toda e qualquer definição acerca dos dados: como acessa-los, como valida-los, seus comportamentos e quais relacionamentos existem entre os mesmo
- View: a camada intermediaria. Camada que associa modelos a templates. Podem conter rergas de negocios implementadas
- Template: camada de apresentação. Essa camada contem as decisoes relacionadas a apresentação: como algo deve ser apresentado na pagina web ou outro tipo de documento
### Principais caracteristicas
- URls amigaveis: permite a criação de urls de maneira simples e que tenham aparecenia amigavel
- sistemas de cache: o framework possui um sistema 

## Unified modeling language - UML
- O desenvolvimento de um software feve seguir algumas etapas para garantinr qualidade, reduzir as chances de erros e facilitar o trabalho dos envolvidos, é preciso elaborar um documentação contendo a estrutura do projeto
- Isso pode ser feito com a UML, uma linguagem de notação essencial em varias etapas da criação de um produtop de software orientado a objetos, utilizando uma serie de elementos graficos.
### Diagramas estruturais
- modelam aspectos estaticos do software, como metodos, interfaces, serviços, arquiteturas, e classes, por exemplo
- ex: diagrama de classe, diagrama de componentes, diagrama de implantação, diagramas de objetos, diagramas de pacotes, etc
### DIagramas comportamentais
- especificam detalhes do comportamento do software, demsontrando o que deve acontecer no sistema
- ex: diagrama de caso de uso, diagrama de atividades, diagrama de maqiuna de estado, diagrama de sequencia, etc