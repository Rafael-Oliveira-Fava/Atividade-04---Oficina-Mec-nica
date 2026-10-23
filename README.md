# Sistema de Gestão de Oficina Mecânica 🚗⚙️

Sistema web simples e eficiente para gerenciamento de clientes, veículos e agendamentos de serviços em oficina mecânica, desenvolvido com Flask e MySQL.

---

## 🚀 Funcionalidades

- **Autenticação:** Login de usuários com controle de sessão e tempo de expiração automático.
- **Gestão de Clientes:** Cadastro e edição de clientes com busca integrada e armazenamento seguro de CPF (`bcrypt`) em conformidade com a LGPD.
- **Gestão de Veículos:** Cadastro e associação de veículos a clientes cadastrados.
- **Agendamentos:** Listagem ordenada por data com detalhes do veículo e cliente, permitindo atualização de datas e status.

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3.10+
- **Framework Web:** Flask
- **Banco de Dados:** MySQL
- **Segurança:** Bcrypt

---

## 📋 Pré-requisitos

- Python 3.10+ instalado
- MySQL Server ativo

---

## 🔧 Como Executar o Projeto

1. **Clonar o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/oficina-mecanica.git
   cd oficina-mecanica
   ```

2. **Criar e ativar o ambiente virtual:**
   ```bash
   python -m venv venv
   
   # Linux/macOS:
   source venv/bin/activate

   # Windows:
   venv\Scripts\activate
   ```

3. **Instalar as dependências:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configurar o Banco de Dados:**
   - Importe o script `db.sql` no MySQL para criar a base e dados de teste:
     ```bash
     mysql -u root -p < db.sql
     ```
   - Caso precise alterar as credenciais do banco, ajuste o arquivo `db.py` ou defina as variáveis de ambiente (`DB_HOST`, `DB_USER`, `DB_PASSWORD`, etc.).

5. **Executar a aplicação:**
   ```bash
   python app.py
   ```
   Acesse em seu navegador: `http://localhost:5000`

---

## 🔑 Credenciais para Teste

| Usuário | Login | Senha |
| :--- | :--- | :--- |
| Administrador | `admin` | `admin123` |
| Carlos Mecânico | `carlos` | `carlos123` |
| Ana Atendente | `ana` | `ana12345` |
