# ⚡ FastAPI CRUD API com Autenticação Básica

Este projeto é uma API simples utilizando **FastAPI**, **Uvicorn** e **Pydantic** para operações CRUD em uma lista de itens, com autenticação básica.

## 🚀 Tecnologias Utilizadas

- [FastAPI](https://fastapi.tiangolo.com/)
- [Uvicorn](https://www.uvicorn.org/)
- [Pydantic](https://pydantic-docs.helpmanual.io/)

## 📁 Estrutura

- `main.py`: Código principal com rotas da API e autenticação básica.
- `requirements.txt`: Dependências necessárias para rodar o projeto.

## ⚙️ Como Executar


1. Crie e ative um ambiente virtual:

```bash
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate
```

2. Instale as dependências:

```bash
pip install -r requirements.txt
```

3. Inicie o servidor:

```bash
uvicorn main:app --reload
```

4. Acesse a documentação interativa (Swagger UI):

```
http://localhost:8000/docs
```

Ou a documentação alternativa (ReDoc):

```
http://localhost:8000/redoc
```

## 🔐 Autenticação

Alguns endpoints exigem autenticação básica HTTP.

- **Usuários disponíveis:**
  - `user1` / `password1`
  - `user2` / `password2`

Use esses usuários ao testar rotas protegidas, como `/hello`.

## 📌 Endpoints Principais

- `GET /` → Página inicial simples.
- `GET /hello` → Saudação autenticada.
- `GET /items` → Lista todos os itens.
- `POST /items` → Cria um novo item.
- `PUT /items/{item_id}` → Atualiza um item existente.
- `DELETE /items/{item_id}` → Remove um item existente.

## 📝 Licença

MIT
