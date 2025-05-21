# trabalho-containers

Este repositório contém uma API desenvolvida em Go (Golang) com foco na aplicação da **Clean Architecture** e conteinerização.

# 👤 Integrantes do Grupo

Bernardo Sozo Fattini, Gabriel Brocco de Oliveira, Gabriel Pradegan Orsatto, Jean Folle Vanz, Otávio Augusto Lorezatto

## 📌 Objetivo

O objetivo deste projeto é implementar um CRUD simples e demonstrar como estruturar uma aplicação de forma organizada e desacoplada, colocando em prática a arquitetura hexagonal (Ports and Adapters) no desenvolvimento de APIs com Go.

## 📁 Estrutura do Projeto

- `cmd/` — Ponto de entrada da aplicação.
- `internal/` — Contém a lógica de negócio e domínios internos.
- `pkg/di/` — Responsável pela injeção de dependências.
- `Dockerfile` e `docker-compose.yaml` — Para facilitar o deploy da aplicação em containers.

## 🚀 Tecnologias Utilizadas

- Go
- PostgresSQL
- Docker Compose

## 📚 Bibliotecas Utilizadas

- pq - github.com/lib/pq – Driver PostgreSQL para Go.

- chi - github.com/go-chi/chi – Um router leve e rápido para construção de APIs HTTP em Go.

- migrate - github.com/golang-migrate/migrate – Ferramenta de migração de banco de dados.

- Viper - github.com/spf13/viper – Biblioteca para configuração de aplicações (JSON, TOML, YAML, env, etc).

## ▶️ Como Executar

Clone o repositório, instale as dependências e utilize o Docker para subir a aplicação:

```bash
git clone https://github.com/gaabrielbrocco/trabalho-containers.git
cd trabalho-containers
go mod tidy
docker compose up --build -d
