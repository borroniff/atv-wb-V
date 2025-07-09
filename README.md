# Sistema de Gerenciamento WB - Full Stack

## 📋 Descrição
Sistema completo para o Grupo World Beauty, contendo:
- **Backend**: API RESTful em Node.js com Express e MySQL
- **Frontend**: Aplicação Next.js com React e TypeScript
- **Relatórios**: Sistema avançado de geração de relatórios

## 🚀 Tecnologias

### Backend
- **Node.js**: 18.x
- **Express**: 5.x
- **MySQL2**: 3.x
- **CORS**: 2.x

### Frontend
- **Next.js**: 15.3
- **React**: 19
- **TypeScript**: 5
- **Tailwind CSS**: 4

## ✅ Funcionalidades

### Backend
- CRUD completo para:
  - Clientes
  - Produtos 
  - Serviços
- Sistema de relatórios:
  - Top 10 clientes (maior/menor consumo)
  - Top 5 clientes (maior valor)
  - Consumo por gênero
  - Produtos/serviços mais consumidos

### Frontend
- Interface moderna e responsiva
- Formulários de cadastro/edição
- Listagens completas
- Visualização de relatórios
- Navegação intuitiva

## 🛠️ Como executar

### Pré-requisitos
- Node.js 18.x ou superior
- MySQL instalado e configurado

### Configuração do Banco de Dados
1. Acesse o MySQL:
```bash
mysql -u root -p
```

2. Crie o banco de dados e usuário:
```sql
CREATE DATABASE world_beauty;
CREATE USER 'app_user'@'localhost' IDENTIFIED BY 'SenhaSegura@123';
GRANT ALL PRIVILEGES ON world_beauty.* TO 'app_user'@'localhost';
FLUSH PRIVILEGES;
```

### Backend
1. Configure o ambiente:
```bash
cd backend
touch .env
```

2. Edite o arquivo `.env`:
```env
DB_HOST=localhost
DB_USER=app_user
DB_PASSWORD=SenhaSegura@123
DB_NAME=world_beauty
PORT=3001
```

3. Instale e execute:
```bash
npm install
npm start
# ou para desenvolvimento:
npm run dev
```

### Frontend
1. Instale e execute:
```bash
cd frontend
npm install
npm run dev
```

## 📂 Estrutura do Projeto

### Backend
```
backend/
├── src/
│   ├── controllers/      # Lógica dos endpoints
│   ├── database/         # Configuração do banco
│   ├── routes/           # Definição das rotas
│   └── index.js          # Ponto de entrada
```

### Frontend
```
frontend/
├── src/
│   ├── app/              # Páginas da aplicação
│   ├── components/       # Componentes reutilizáveis
│   │   ├── Forms/        # Formulários
│   │   └── Table/        # Componentes de tabela
│   └── types/            # Tipos TypeScript
```

## 👨‍💻 Desenvolvido por
Angelina Borroni Ferreira
