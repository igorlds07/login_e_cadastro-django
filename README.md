# Desafio Técnico - Sistema de Login e Cadastro

## 📝 Descrição

O sistema permite que os usuários se cadastrem, façam login, e sejam redirecionados para uma tela de **Menu** após o login bem-sucedido. Ele inclui validações para garantir que os dados sejam inseridos corretamente (como e-mail válido, senhas fortes e a confirmação da senha).

Além disso, após o cadastro, um e-mail de confirmação é enviado para o usuário informando sobre o sucesso no registro.

## 🚀 Funcionalidades

- **Tela de Login**:  
    - Validação de e-mail e senha.
    - Mensagens de erro claras para quando o e-mail ou senha estiverem errados.
    - Redirecionamento para a tela de Menu após o login bem-sucedido.
  
- **Tela de Registro**:  
    - Campos de **nome**, **e-mail**, **senha** e **confirmar senha**.
    - Validação de:
        - Nome de usuário (apenas letras).
        - E-mail válido.
        - Senha com pelo menos 8 caracteres, 1 letra maiúscula, 1 número e 1 caractere especial.
        - A confirmação da senha.
    - Envio de e-mail de confirmação para o usuário após o registro.

## 🧑‍💻 Como Usar

1. **Clonar o repositório:**

   Abra o terminal e digite:

   ```bash
   git clone https://github.com/igorlds07/login_e_cadastro-django
   
Instalar as dependências:
Certifique-se de estar no diretório do projeto e tenha um ambiente virtual Python ativado. Execute o seguinte comando:
pip install -r requirements.txt


Configuração do Banco de Dados:
Para configurar o banco de dados (SQLite por padrão), rode o comando:
python manage.py migrate


Para rodar a aplicação localmente, use:

python manage.py runserver

O sistema estará disponível em http://127.0.0.1:8000.


Criar um superusuário (opcional):

Se você quiser criar um superusuário para acessar o painel de administração, basta rodar:
python manage.py createsuperuser
Depois, basta acessar o painel admin em http://127.0.0.1:8000/admin/.

🛠 Tecnologias Usadas
Django : Framework web Python utilizado para desenvolver a aplicação.
SQLite : Banco de dados relacional simples utilizado para armazenar as informações dos usuários.
Email : Envio de e-mails de confirmação após o cadastro.


🧩 Estrutura do Projeto
O projeto é organizado da seguinte maneira:

/desafio-login
    ├── /cadastro/                 # Tela de registro de usuários
    ├── /login/                    # Tela de login
    ├── /menu/                     # Tela de menu após login
    ├── /templates/                # Arquivos HTML
    ├── /static/                   # Arquivos estáticos (CSS, JS, imagens)
    └── /migrations/               # Migrations do banco de dados

    
✨ Melhorias Futuras
Validação de E-mail Real : Envia um link de ativação para confirmar o e-mail.
Melhorias no design : Implementação de um design mais interativo e visual.
Segurança : Implementação de funcionalidades como autenticação multifatorial (2FA).
Funcionalidades do Menu : Adicione novas funcionalidades à tela do menu, como editar dados do usuário.
