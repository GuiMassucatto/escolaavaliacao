# Avaliação Prática: Sistema de Turmas e Atividades

### Objetivo
Este projeto tem como meta desenvolver uma **aplicação web completa** (back-end e front-end) voltada ao gerenciamento de turmas e atividades de professores.  
O sistema permite que o docente cadastre, visualize e remova turmas e atividades de forma simples e centralizada.  

### Cenário
Em diversas instituições, principalmente nas regiões mais afastadas, a ausência de ferramentas digitais adequadas compromete a organização das atividades pedagógicas.  
Um sistema que facilite o acompanhamento do conteúdo aplicado e avaliado contribui para a eficiência e continuidade do processo de ensino-aprendizagem.

### Tarefa
Criar uma aplicação funcional que possibilite ao professor:
- Realizar login com credenciais seguras;
- Registrar, consultar e remover turmas cadastradas;
- Cadastrar atividades vinculadas às turmas;
- Efetuar logout com segurança.

---

## Requisitos Técnicos do Ambiente

Para executar o sistema corretamente, o ambiente de desenvolvimento deve atender às seguintes especificações:

### 1. Banco de Dados
- **SGBD:** MySQL  
- **Versão recomendada:** 8.0 ou superior  
- **Observação:** Criar um banco de dados específico para o projeto com usuário e senha configurados.

### 2. Servidor / Sistema Operacional
- **Sistema Operacional:** Windows 10/11, Linux (Ubuntu 20.04 ou superior) ou macOS  
- **Sistema Operacional:** Windows 10/11
- **Servidor de Aplicação:** Node.js  
- **Versão recomendada do Node.js:** 18.x ou superior
- **Versão recomendada do Node.js:** 18 ou superior

### 3. Linguagens e Frameworks
- **Back-end:** JavaScript (Node.js, Express, Prisma ORM)  
@@ -37,3 +37,53 @@


---

## Passo a Passo de Instalação e Execução

Siga as instruções abaixo para preparar e executar o sistema localmente:

### 1. Clonar o Repositório

```bash
git clone https://github.com/GuiMassucatto/escolaavaliacao.git
cd escolaavaliacao
```

### 2. Instalar Dependências

```bash
npm install
ou
npm i
```

### 3. Configurar Banco de Dados
- Crie um banco de dados MySQL específico para o projeto.  
- Configure o `.env`:

```env
DATABASE_URL="mysql://root@localhost:3306/nome_do_banco"
```

### 4. Rodar Migrations do Prisma

```bash
npx prisma migrate dev --name init
```

### 5. Iniciar o Servidor

```bash
npm run dev
```

O servidor estará disponível em `http://localhost:3000`.

### 6. Testar o Sistema
- Acesse pelo navegador ou utilize o **Insomnia/Postman** para testar a API.  
- Funcionalidades para testar:
  - Cadastro, listagem, edição e exclusão de turmas;
  - Cadastro, listagem, edição e exclusão de atividades;
  - Login e logout do professor.
