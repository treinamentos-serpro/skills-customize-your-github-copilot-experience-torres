# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Construa uma API REST em Python usando FastAPI para gerenciar tarefas. Ao concluir, você terá praticado criação de rotas, validação de dados com modelos, operações CRUD e uso adequado de códigos de status HTTP.

## 📝 Tasks

### 🛠️ Criar a API e listar tarefas

#### Descrição
Configure uma aplicação FastAPI para gerenciar tarefas e implemente a rota inicial para consultar todas as tarefas.

#### Requisitos
O programa concluído deve:

- Criar uma aplicação FastAPI executável com Uvicorn
- Implementar `GET /tasks`, retornando uma lista vazia quando ainda não houver tarefas
- Disponibilizar a documentação interativa da API em `/docs`


### 🛠️ Criar e consultar tarefas

#### Descrição
Defina um modelo para representar uma tarefa e implemente as rotas para criar uma tarefa e consultar uma tarefa pelo identificador.

#### Requisitos
O programa concluído deve:

- Definir um modelo `Task` com `id`, `title`, `description` e `completed`
- Exigir `title` e usar `false` como valor padrão de `completed`
- Implementar `POST /tasks`, retornando a tarefa criada com o status HTTP `201`
- Implementar `GET /tasks/{task_id}`, retornando `404` quando o identificador não existir


### 🛠️ Atualizar e remover tarefas

#### Descrição
Complete as operações CRUD permitindo atualizar e excluir tarefas existentes.

#### Requisitos
O programa concluído deve:

- Implementar `PUT /tasks/{task_id}` para atualizar os dados de uma tarefa existente
- Implementar `DELETE /tasks/{task_id}` para remover uma tarefa existente
- Retornar `404` ao tentar atualizar ou remover uma tarefa inexistente
- Manter os dados em memória durante a execução da aplicação, sem exigir banco de dados