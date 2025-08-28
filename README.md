# 💊 FarmaFacilAPI

API RESTful que **automatiza a gestão** de usuários, produtos e endereços, otimizando operações do sistema FarmaFácil.

---

## 📚 Documentação da API

Após rodar o projeto localmente, a documentação estará disponível em:

👉 [http://localhost:3000/api-docs](http://localhost:3000/api-docs)

---

## 🚀 Tecnologias Utilizadas

- Node.js + Express
- TypeScript
- Prisma (ORM)
- PostgreSQL (banco de dados)
- Swagger (documentação da API)
- JWT (JSON Web Tokens) 


## 🛠️ Como rodar o projeto localmente

### 1. Clone o repositório

```bash
git clone https://github.com/SeuUsuario/FarmaFacilAPI.git
cd FarmaFacilAPI
```

### 2. Instale as dependências
```bash
npm install
```

### 3. Configure as variáveis de ambiente
```bash
DATABASE_URL="postgresql://usuario:senha@localhost:5432/farmafacil"
DEV_MODE=true
PORT=3000
```

### 4. Configure o banco de dados
```bash
npx prisma migrate dev --name init
npx prisma generate
```

### 5. Rode a aplicação
```bash
npm run dev
```

___
📁 Estrutura do Projeto

```bash
src/
├── app/
│   ├── controller/        # Controladores (User, Product, Address)
│   ├── dao/               # Acesso a dados com Prisma
│   └── usecases/          # Casos de uso e regras de negócio
├── core/
│   ├── app.ts             # Configuração principal do Express
│   ├── db.ts              # Conexão com o banco de dados
│   ├── routes.ts          # Definição das rotas
│   └── swagger.ts         # Configuração da documentação Swagger
└── prisma/
    └── schema.prisma      # Schema do banco de dados

```

___
✅ Funcionalidades

    Cadastro e login de usuários

    CRUD de produtos

    Busca de produtos por código, categoria e últimos adicionados

    CRUD de endereços

    Geração e remoção de seeds (modo dev)

    Busca de usuários por email
    
    Atualização de estoque de produtos 
    
___
👥 Contribuição

Para contribuir:

    Faça um fork deste repositório

    Crie uma branch: git checkout -b minha-feature
    Use mensagens de commit claras e no imperativo (ex: "Adiciona X", "Corrige Y").  

    Faça suas alterações e commit: git commit -m '[FEAT] Minha nova feature'

    Inclua testes unitários para suas alterações.  <--- SUA ALTERAÇÃO AQUI

    Push: git push origin minha-feature

    Abra um Pull Request
=======
# FarmaFacil
para rodar a aplicação backend basta rodar os comandos  
npm i  
npm run dev
