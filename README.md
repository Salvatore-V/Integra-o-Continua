Projeto de Aplicação Web em Go com Integração Contínua

Este projeto consiste numa aplicação web desenvolvida em Go (Golang) estruturada sob o padrão MVC, focada na implementação de práticas de Integração Contínua (CI) utilizando o GitHub Actions.

Tecnologias e Ferramentas Utilizadas

Linguagem Backend: Go (Golang)

Base de Dados: PostgreSQL (gerida via Docker Compose)

Automação / CI: GitHub Actions (.github/workflows/go.yml)

Contêineres: Docker e Docker Compose

Automação de Tarefas: Makefile


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
