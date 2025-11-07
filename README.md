# 📄 Relatório de Projeto Galesmy (GRUPO 12)
## Identificação do Grupo
- **Ari Manuel Gamboa Aguilar** – USP nº 16796572  
- **Sandro Fabrizio Cárdenas Vilca** – USP nº 16796589  

## 1. Descrição do Projeto 

### 1.1. Telas Funcionais

| Página                      | Descrição                                                                 |
|----------------------------|---------------------------------------------------------------------------|
| `homepage.html`            | Tela inicial com apresentação da loja e acesso a login                    |
| `loginpage.html`           | Autenticação de usuários com redirecionamento por perfil                  |
| `register.html`            | Formulário de registro com máscaras e validações                         |
| `Produtos_Page.html`       | Catálogo de produtos com filtro por categoria                            |
| `Produto_Individual.html`  | Página de detalhes de produto com botão de compra                         |
| `carrito_compras.html`     | Carrinho de compras interativo com resumo                                |
| `pagamento.html`           | Finalização do pedido e geração da boleta em PDF                         |
| `usuario.html`             | Visualização e edição do perfil do cliente                               |
| `contactopage.html`        | Formulário de contato funcional                                          |

### 1.2. Telas Administrativas

| Página                      | Função                                                                 |
|----------------------------|------------------------------------------------------------------------|
| `admin-productos.html`     | Listagem e gerenciamento de produtos                                   |
| `admin-add-product.html`   | Cadastro de novo produto                                               |
| `admin-edit-product.html`  | Edição de produto existente                                            |
| `admin-usuarios.html`      | Lista de clientes e admins registrados                                |
| `admin-add-admin.html`     | Cadastro de novo administrador                                         |
| `admin-edit-user.html`     | Edição de dados de um usuário  
---
---

## 2. Backend: Estrutura e Tecnologias

### 📁 Estrutura

```
backend/
├── .env                     # String de conexão com MongoDB Atlas
├── models/
│   ├── Produto.js           # Esquema do Produto (Mongoose)
│   └── Usuario.js           # Esquema do Usuário (Mongoose)
├── routes/
│   ├── produtos.js          # Rotas GET, POST, PUT, DELETE para produtos
│   ├── usuarios.js          # Autenticação, criação e edição de usuários
│   └── initUser.js          # Cria admin inicial se não existir
├── server.js                # Inicialização do servidor Express
├── package.json             # Dependências e scripts
```

### 🧠 Tecnologias Usadas

- **Node.js + Express**: servidor e rotas
- **MongoDB Atlas**: banco de dados NoSQL na nuvem
- **Mongoose**: ODM para modelar dados
- **dotenv**: carregamento da string de conexão segura
- **CORS e JSON Middleware**: configuração do Express para lidar com requisições web

---

## 3. Funcionalidades Completas

| Funcionalidade                          | Status |
|-----------------------------------------|--------|
| Login com sessão                        | ✅     |
| Redirecionamento por tipo de usuário    | ✅     |
| CRUD completo de produtos (MongoDB)     | ✅     |
| CRUD completo de usuários (MongoDB)     | ✅     |
| Carrinho funcional                      | ✅     |
| Geração de boleta                       | ✅     |
| Formulário de contato funcional         | ✅     |
| Autenticação com email/senha            | ✅     |
| Admin inicial criado automaticamente    | ✅     |
| Atualização de estoque após compra      | ✅     |

---
## 4. Plano de Testes

**Testes manuais realizados:**

- Login e redirecionamento de usuários.
- Renderização de produtos e filtro por categoria.
- Manipulação completa do carrinho.
- Geração de boleta em PDF com produtos corretos.
- CRUD de produtos e usuários.
- Teste de envio de mensagens pelo formulário de contato.
- Máscaras aplicadas corretamente nos campos dos formulários.

---

## 5. Resultados dos Testes

Todos os testes foram executados com sucesso. As funcionalidades estão operacionais com resultados consistentes. Nenhum bug crítico foi identificado.

| Funcionalidade                         | Status |
|----------------------------------------|--------|
| Login de cliente/admin                 | ✅     |
| Redirecionamento por tipo de usuário   | ✅     |
| Carrinho com total dinâmico            | ✅     |
| CRUD de produtos e usuários            | ✅     |
| Geração de boleta                      | ✅     |
| Formulário “Contate-nos”               | ✅     |
| Máscara de CPF/telefone                | ✅     |
| Sessão e nome do usuário logado        | ✅     |
| Filtro por categoria                   | ✅     |
| SPA parcial com navegação              | ✅     |

---
## 6. Baixar o projeto para sua máquina
**Download ZIP**

- Na página do GitHub → botão Code → Download ZIP.
- Descompacte você obterá 2 arquivos (Galesmy.zip e README.md)
- Descompacte Galesmy.zip, você obterá a pasta Galesmy
- A pasta Galesmy abra no VS Code.
---
## 7. Execução

## 1) 📥 No VS Code, abra um terminal (Ctrl + ç) e vá para a pasta “backend”:
```bash
cd backend
```

## 2) 📦 Instale as dependências do backend:
```bash
npm install
```
## 3) ▶️ Rodar o servidor

```bash
node server.js
```

Você verá no terminal:

```
🚀 Servidor rodando na porta 3000: http://localhost:3000
✅ Conectado a MongoDB Atlas
```

---
## 8. Usuário Administrador Padrão
Foi criado automaticamente um admin padrão na coleção `usuarios`:

```txt
Email: galesmy@empresa.com
Senha: admin123
```
---

## ✅ Check de Requisitos Finais

| Item                                                     | Ok |
|----------------------------------------------------------|----|
| Backend com Node.js e Express                            | ✅ |
| Conexão com MongoDB Atlas                                | ✅ |
| Código bem comentado e formatado                         | ✅ |
| API funcional com rotas para usuários e produtos          | ✅ |
| Relatório atualizado com este milestone final            | ✅ |
| Projeto completo no GitHub                               | ✅ |
