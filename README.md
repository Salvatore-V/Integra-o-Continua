Projeto de Aplicação Web em Go com Integração Contínua

Este projeto consiste numa aplicação web desenvolvida em Go (Golang) estruturada sob o padrão MVC, focada na implementação de práticas de Integração Contínua (CI) utilizando o GitHub Actions.

Tecnologias e Ferramentas Utilizadas

Linguagem Backend: Go (Golang)

Base de Dados: PostgreSQL (gerida via Docker Compose)

Automação / CI: GitHub Actions (.github/workflows/go.yml)

Contêineres: Docker e Docker Compose

Automação de Tarefas: Makefile

Estrutura do Projeto

3983-integracao-continua-main/
├── .github/workflows/      # Pipeline de Integração Contínua (go.yml)
├── assets/                 # Folhas de estilo CSS (index.css, 404.css)
├── controllers/            # Lógica de controlo de requisições (controller.go)
├── database/               # Configuração e conexão com a base de dados (db.go)
├── models/                 # Definição de estruturas e dados (alunos.go)
├── routes/                 # Mapeamento de rotas da aplicação (route.go)
├── templates/              # Páginas HTML da interface (index.html, 404.html)
├── docker-compose.yml      # Orquestração de serviços e base de dados PostgreSQL
├── Makefile                # Automação de comandos locais
├── main.go                 # Ponto de entrada da aplicação
└── main_test.go            # Testes automatizados da aplicação


Principais Casos Implementados e Funcionalidades

A aplicação gere operações web orientadas a estudantes, contando com:

Gestão de Rotas e Controladores: Arquitetura limpa para processamento de rotas e renderização de templates HTML.

Persistência de Dados: Integração com PostgreSQL gerida através de contentores Docker.

Pipeline de CI/CD: Configuração automatizada para execução de testes e validação contínua do código a cada atualização no repositório.

Como Executar o Projeto Localmente.

Pré-requisitos: Certifique-se de ter o Go, Docker e Docker Compose instalados na sua máquina.

Subir os Serviços (Base de Dados):

docker-compose up -d


Executar a Aplicação:

go run main.go
