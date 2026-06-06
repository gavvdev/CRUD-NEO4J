# 🎬 CRUD de Filmes com Neo4j

Este é um projeto simples de CRUD (Create, Read, Update, Delete) em **Python**, que utiliza o **Neo4j** como banco de dados orientado a grafos. O menu é interativo via terminal e permite gerenciar filmes com título e ano de lançamento.

---

## 💾 Pré-requisitos

- Python 3.10+
- Neo4j rodando localmente ou em nuvem
- Variáveis de ambiente configuradas em um arquivo `.env`

---

## 📦 Instalação

```bash
# Clone o repositório
git clone (nome do repositorio)
cd CRUD-NEO4J

# Crie e ative um ambiente virtual (opcional, mas recomendado)
python -m venv venv
venv\Scripts\activate  # No Windows
# source venv/bin/activate  # No Linux/macOS

# Instale as dependências
pip install -r requirements.txt
```

## 🔐 Configuração
Crie um arquivo chamado .env na raiz do projeto com as seguintes variáveis:
```bash
NEO4J_URI=bolt://localhost:7687
NEO4J_USER=neo4j
NEO4J_PASSWORD=sua_senha
```
⚠️ Não suba esse arquivo para o GitHub. Ele já está no .gitignore.

## ▶️ Executando o programa
```bash
python app.py
```


## 🖥️ Exemplo de uso no terminal
```bash
=== Menu de Filmes ===
1. Criar filme
2. Listar filmes
3. Atualizar filme
4. Deletar filme
5. Sair
Escolha (1-5): 1
Título: Matrix
Ano: 1999
Filme 'Matrix' criado!

Escolha (1-5): 2
Título: Matrix, Ano: 1999

Escolha (1-5): 3
Título atual: Matrix
Novo título: Matrix Reloaded
Novo ano: 2003
Filme 'Matrix' atualizado!

Escolha (1-5): 4
Título para deletar: Matrix Reloaded
Filme 'Matrix Reloaded' deletado!

Escolha (1-5): 5
Saindo...

```
## 🧠 Tecnologias usadas
Python

Neo4j

neo4j driver oficial

python-dotenv para variáveis de ambiente
