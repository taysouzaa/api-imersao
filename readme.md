# 🎓 API de Gestão Escolar | Imersão DevOps - Alura + Google Cloud

Gerencie alunos, cursos e matrículas com uma API REST moderna e escalável

[![FastAPI](https://img.shields.io/badge/Built_with-FastAPI-009688?logo=fastapi)]()
[![Docker](https://img.shields.io/badge/Containerized-Docker-2496ED?logo=docker)]()
[![GCP](https://img.shields.io/badge/Deployed-Google%20Cloud%20Run-4285F4?logo=googlecloud)]()

Desenvolvido durante a **Imersão DevOps da Alura + Google Cloud**, este projeto aplica práticas modernas de desenvolvimento e deploy com foco em escalabilidade, modularidade e produtividade.

---

##  Visão Geral

Esta é uma **API REST** desenvolvida com **FastAPI** para gerenciar:

- 👩‍🎓 Alunos  
- 📚 Cursos  
- 📝 Matrículas  

Além da lógica de aplicação, o projeto abrange:

- ✅ Containerização com Docker  
- ☁️ Deploy na Google Cloud Platform  
- 🧱 Arquitetura modular com routers, models e schemas  
- 🧪 Testes e documentação automática via Swagger  

---

## ✅ Funcionalidades

- CRUD completo de Alunos, Cursos e Matrículas  
- Banco de dados local com **SQLite**  
- Documentação interativa com Swagger  
- Estrutura modular e pronta para escalar  
- Imagens Docker para facilitar deploy e execução  

---

## 🧩 Estrutura do Projeto

```bash

.
├── app.py                # Ponto de entrada da aplicação
├── database.py           # Configuração do banco de dados SQLite
├── routers/              # Rotas organizadas por entidade
├── models.py             # Modelos SQLAlchemy
├── schemas.py            # Schemas de validação (Pydantic)
├── requirements.txt      # Lista de dependências
├── Dockerfile            # Container Docker
├── docker-compose.yml    # (Opcional) Orquestração de containers
└── .gitignore            # Itens ignorados no versionamento
````

---

## 🐳 Executando com Docker

> Certifique-se de ter o Docker instalado:  
🔗 [Instalar Docker](https://www.docker.com/get-started)

# Build da imagem
```bash
docker build -t api-escolar .
````

# Executar o container
```bash
docker run -d -p 8000:8000 api-escolar
````

Acesse a documentação Swagger:
📘 [http://localhost:8000/docs](http://localhost:8000/docs)

---

## ☁️ Deploy na Google Cloud

A API foi implantada na **Google Cloud Run** com escalabilidade automática.
Durante a imersão, foram aplicadas as seguintes práticas:

* Criação de projeto no Google Cloud
* Deploy de imagem via **Google Container Registry**
* Publicação com **Cloud Run** com CI/CD simplificado

---

## 🧪 Execução Local (sem Docker)

> Requisitos:

* Python 3.10+
* Git


# Clone o repositório
```bash
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
```

# Crie e ative o ambiente virtual
```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

# Instale as dependências
```bash
pip install -r requirements.txt
```

# Inicie a aplicação
```bash
uvicorn app:app --reload
```

---

## 🌐 Interface da API

Depois de executar o servidor localmente ou via Docker, acesse:
📘 [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

## 👩‍💻 Desenvolvedora

**Taynara Souza**
📧 [taynara.souza.dev@gmail.com](mailto:taynara.souza.dev@gmail.com)
🔗 [linkedin.com/in/taynara-correia-souza](https://www.linkedin.com/in/taynara-correia-souza)

---

## 📚 Créditos

Este projeto foi desenvolvido durante a **Imersão DevOps** promovida pela **Alura** em parceria com a **Google Cloud**.
Agradecimento especial ao instrutor **Guilherme Lima** pela excelente didática!

---

