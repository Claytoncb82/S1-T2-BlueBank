# S1-T2-BlueBank

<h1 align="center"><a href="https://bancopan.corporate.gama.academy/"><img width="250" height="150"src="https://bancopan.corporate.gama.academy/wp-content/uploads/sites/10/2021/08/logo-Positivo.png"><img width="250" height="150"src="https://bancopan.corporate.gama.academy/wp-content/uploads/sites/10/2021/08/gama-academy-logo-horizontal-verde-preto.png"</a></h1>

#### A PAN Academy juntamente com o Banco Pan fomalizaram o programa para aprimorar o conhecimento em JAVA e Cloud, com uma ementa bem elaborada para os alunos, com aulas diárias e no sábado, formatada para o projeto. Além do conhecimento teórico teremos a aplicação do aprendizado em um Projeto Final.


> Status: 🚀 Em desenvolvimento...  🚧

> ### 🛠 Desenvolvedores da Squad

- [Clayton Cesar Batista](https://github.com/Claytoncb82/)
- [Hanely Taniguchi](https://github.com/Honey-lee429)
- [Marcus Thadeu da Silva Batista](https://github.com/DevMarcus007)
- [Nathan Liyodi Nariai](https://github.com/nyodinariai)

> ### Endpoints

Método    |             URL           |            Finalidade
--------- | ------                    | ----------
GET       | /cliente                  | Lista todos os cliente
GET       | /cliente/{id}             | Lista de um cliente por ID
DELETE    | /cliente/{id}             | Inativa um cliente por ID
PUT       | /cliente/{id}             | Atualiza um cliente por ID
POST      | /cliente/cadastrar        | Adiciona um novo cliente
POST      | /cliente/logar            | Acessa a conta do cliente
GET       | /conta                    | Lista todas as contas
GET       | /conta/{id}               | Lista conta por ID
DELETE    | /conta/{id}               | Inativa conta por ID
POST      | /conta/criar              | Adiciona uma nova conta
GET       | /conta/movimentacoes/{id} | Lista movimentação da conta por ID
GET       | /conta/conta/saldo/{id}   | Lista saldo da conta por ID
GET       | /movimentacoes            | Lista todas movimentações
POST      | /movimentacoes/depositar  | Realiza um depósito em conta
POST      | /movimentacoes/sacar              | Realiza um saque em conta
POST      | /movimentacoes/transferir/{id}    | Realiza uma movimentação entre contas
  
  


> ### 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

- [Eclipse](https://www.eclipse.org/)
- [SQL]()
- [Java]()
- [MySQL]()
- [Amazon Web Service]()
- [Jira](https://www.atlassian.com/br/software/jira/)
- [Main Repository]()
- [Xampp]()

  
> ### 🛠 Estrutura de Diretórios  
  
  ```shell
└───apibluebank  
    │   .gitignore  
    │   api-spring-aws.iml  
    │   buildspec.yml  
    │   mvnw  
    │   mvnw.cmd  
    │   pom.xml  
    │   README.md   
    └───src  
        ├───main  
        │   ├───java  
        │   │   └───api  
        │   │       └───spring  
        │   │           └───bluebank  
        │   │               │   ApibluebankApplication.java  
        │   │               │   buildspec.yml  
        │   │               │  
        │   │               ├───configuration  
        │   │               │       SwaggerConfig.java  
        │   │               │  
        │   │               ├───controller  
        │   │               │       ClienteController.java  
        │   │               │       ContaController.java  
        │   │               │       MovimentacoesController.java  
        │   │               │  
        │   │               ├───exception  
        │   │               │       NaoEcontrado.java  
        │   │               │  
        │   │               ├───model  
        │   │               │   │   Cliente.java  
        │   │               │   │   Conta.java  
        │   │               │   │   Endereco.java  
        │   │               │   │   Movimentacoes.java  
        │   │               │   │   TipoCliente.java  
        │   │               │   │  
        │   │               │   └───enun  
        │   │               │           TipoCliente.java  
        │   │               │           TipoConta.java  
        │   │               │           TipoMovimentacao.java  
        │   │               │           UF.java  
        │   │               │  
        │   │               ├───repository  
        │   │               │       ClienteRepository.java  
        │   │               │       ContaRepository.java  
        │   │               │       MovimentacoesRepository.java  
        │   │               │  
        │   │               ├───security  
        │   │               │       BasicSecurityConfig.java  
        │   │               │       UserDetailsImplements.java  
        │   │               │       UserDetailsServiceImplements.java  
        │   │               │  
        │   │               └───service  
        │   │                       ClienteService.java  
        │   │                       ContaService.java  
        │   │                       MovimentacoesService.java  
        │   │  
        │   └───resources  
        │           application.properties  
        │  
        └───test  
            └───java  
                └───api  
                    └───spring  
                        └───bluebank  
                                ApibluebankApplicationTests.java  
