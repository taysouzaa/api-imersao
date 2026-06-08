# API de Gestão Escolar

> API REST moderna para gerenciamento de alunos, cursos e matrículas — desenvolvida na Imersão DevOps da Alura + Google Cloud.

![Status](https://img.shields.io/badge/status-concluído-22c55e)
![Python](https://img.shields.io/badge/backend-Python%2FFastAPI-1f6feb)
![Docker](https://img.shields.io/badge/infra-Docker%2FCloud%20Run-0f766e)
![License](https://img.shields.io/badge/license-MIT-green)

## Visão do Projeto

Projeto desenvolvido durante a **Imersão DevOps da Alura + Google Cloud**, aplicando práticas modernas de desenvolvimento, containerização e deploy em nuvem. A API gerencia entidades escolares com endpoints RESTful e banco de dados relacional.

### O que o sistema resolve

- Gerencia alunos, cursos e matrículas via API REST.
- Containeriza a aplicação com Docker para portabilidade total.
- Faz deploy automatizado no Google Cloud Run.

## O Que Foi Desenvolvido

### 1. API REST com FastAPI
- CRUD completo de alunos, cursos e matrículas.
- Validação automática de dados com Pydantic.
- Documentação interativa via Swagger UI (`/docs`).

### 2. Banco de Dados
- SQLite local para desenvolvimento (`escola.db`).
- Models e schemas separados por responsabilidade.
- Roteamento modular por entidade.

### 3. Containerização e Deploy
- `Dockerfile` para build da imagem.
- `Docker-compose.yml` para execução local completa.
- Configurado para deploy no **Google Cloud Run**.

## Stack Técnica

- **Backend:** Python 3, FastAPI, Pydantic
- **Banco:** SQLite (dev)
- **Infra:** Docker, Docker Compose, Google Cloud Run
- **CI/CD:** GitHub Actions (`.github/workflows`)

## Estrutura do Projeto

```text
.
├─ app.py              ← entrypoint da aplicação
├─ database.py         ← configuração do banco
├─ models.py           ← modelos SQLAlchemy
├─ schemas.py          ← schemas Pydantic
├─ routers/            ← endpoints por entidade
├─ requirements.txt    ← dependências Python
├─ Dockerfile
├─ Docker-compose.yml
└─ .github/            ← pipelines CI/CD
```

## Como Executar

```bash
# Com Docker Compose
docker-compose up --build

# Sem Docker
pip install -r requirements.txt
uvicorn app:app --reload
```

Acesse a documentação em: `http://localhost:8000/docs`

## Licença

MIT — veja [LICENSE](./LICENSE)