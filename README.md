# Vellux Motors

## 🛠️ Tecnologias Utilizadas

### Frontend
* **[React](https://react.dev/):** Biblioteca principal para construção da interface.
* **[Vite](https://vitejs.dev/):** Bundler super rápido para desenvolvimento e build.
* **[Tailwind CSS v4](https://tailwindcss.com/):** Framework de CSS utilitário para estilização rápida e responsiva.

### Backend
* **[Node.js](https://nodejs.org/):** Ambiente de execução JavaScript server-side.
* **[Express](https://expressjs.com/):** Framework minimalista para criação da API REST.
* **[pg](https://node-postgres.com/):** Driver nativo para comunicação com o banco de dados.

### Infraestrutura & Dados
* **[PostgreSQL 15](https://www.postgresql.org/):** Banco de dados relacional robusto.
* **[Docker](https://www.docker.com/) & Docker Compose:** Conteinerização e orquestração dos serviços.

---

## 📂 Estrutura do Projeto (Monorepo)

```text
meu-projeto-web/
├── frontend/             # Aplicação React + Tailwind
│   ├── src/              # Código fonte do frontend
│   ├── Dockerfile        # Configuração da imagem do frontend
│   └── vite.config.js    # Configurações do Vite (com suporte a Hot Reload no Docker)
├── backend/              # API Node.js + Express
│   ├── index.js          # Ponto de entrada da API
│   ├── Dockerfile        # Configuração da imagem do backend
│   └── package.json      # Dependências e scripts (ex: node --watch)
├── docker-compose.yml    # Orquestração de todos os serviços (Front, Back, DB)
└── README.md             # Documentação do projeto
```

---

## ⚙️ Pré-requisitos

Para rodar este projeto na sua máquina, você precisará ter instalado:
* [Git](https://git-scm.com/)
* [Docker](https://www.docker.com/products/docker-desktop/) e Docker Compose

---

## 🚀 Como Executar o Projeto

**1. Clone o repositório**
```bash
git clone https://github.com/TPPS-LDPGAutoPecas/SiteVellux.git
cd nome-do-repo
```

**2. Suba os containers com o Docker Compose**
Na raiz do projeto, execute o comando abaixo para construir as imagens e subir os serviços. O processo pode levar alguns minutos na primeira vez.
```bash
docker-compose up --build
```

**3. Acesse a aplicação**
* **Frontend:** [http://localhost:5173](http://localhost:5173)
* **Backend (API):** [http://localhost:3000](http://localhost:3000)
* **Banco de Dados:** Disponível na porta `5432` localmente (User: `admin` | Pass: `adminpassword` | DB: `meubanco`)

---
