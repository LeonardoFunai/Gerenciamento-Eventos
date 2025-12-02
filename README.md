# 🎉 Gerenciador de Eventos (Desafio Proponto)

![PHP](https://img.shields.io/badge/PHP-8.2-777BB4?style=for-the-badge&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-11-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)

> 🏆 **Status:** Projeto Aprovado!
> Este sistema foi desenvolvido como parte do processo seletivo para a vaga de Estágio na **Proponto**, resultando na minha contratação. O objetivo foi demonstrar conhecimentos em arquitetura MVC, CRUD, validações e construção de interfaces responsivas.

---

## 📖 Sobre o Projeto

O **Gerenciador de Eventos** é uma aplicação web robusta desenvolvida em Laravel que permite o controle completo do ciclo de vida de eventos. O sistema foi projetado para ser intuitivo e funcional, garantindo que o usuário possa organizar eventos sociais, corporativos e esportivos com facilidade.

### 🎯 Destaques Técnicos
* **Arquitetura MVC:** Separação clara entre Lógica (Controllers), Dados (Models) e Visualização (Blade Views).
* **Validação Avançada:** Uso de `FormRequests` para garantir a integridade dos dados no back-end.
* **Filtros Dinâmicos:** Implementação de query scopes para filtrar eventos por nome, tipo e intervalo de datas.
* **UX/UI:** Interface limpa construída com Bootstrap 5 e CSS personalizado.

---

## 📸 Screenshots

### 🏠 Dashboard Inicial
*Uma landing page visualmente agradável com acesso rápido às funcionalidades principais.*
![Página Inicial](screenshots/inicio.png)

### 📋 Listagem e Filtragem
*Tabela responsiva com sistema de busca avançada (por período, tipo e nome) e paginação.*
![Listagem de Eventos](screenshots/lista.png)

### 📝 Cadastro de Evento
*Formulário estilizado com validação de campos obrigatórios e máscaras.*
![Cadastro](screenshots/cadastrar.png)

### 🔍 Detalhes do Evento
*Visualização completa das informações, incluindo link direto para o Google Maps.*
![Visualizar Evento](screenshots/visualizar.png)

---

## 🚀 Funcionalidades

✅ **CRUD Completo:** Criação, Leitura, Atualização e Exclusão de eventos.
✅ **Sistema de Filtros:**
   - Busca textual por nome do evento.
   - Filtro por categoria (Social, Esportivo, Cultural, etc.).
   - Filtro por intervalo de datas (Data inicial e final).
✅ **Integração com Mapas:** Campo dedicado para links do Google Maps.
✅ **Feedback ao Usuário:** Alertas visuais (Flash Messages) para confirmar ações de sucesso ou erro.
✅ **Responsividade:** Layout adaptável para desktop e mobile.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** PHP 8.2+
* **Framework:** Laravel 11
* **Front-end:** Blade Templates, Bootstrap 5, Sass
* **Build Tool:** Vite
* **Banco de Dados:** MySQL
* **Gerenciador de Pacotes:** Composer & NPM

---

## 📥 Instalação e Configuração

Siga os passos abaixo para rodar o projeto em seu ambiente local:

### 1️⃣ Clone o Repositório
```bash
git clone [https://github.com/seu-usuario/gerenciamento-eventos.git](https://github.com/seu-usuario/gerenciamento-eventos.git)
cd gerenciamento-eventos

### 🔹 2️⃣ Instale as Dependências  

Instale os pacotes PHP e as dependências frontend:

```bash
composer install
npm install
```

### 🔹 3️⃣ Configuração do Banco de Dados  

1. Crie um banco de dados no MySQL, por exemplo, **event_manager**.
2. Copie o arquivo de exemplo de configuração:

```bash
cp .env.example .env
```

3. Edite o arquivo **.env** e configure as credenciais do banco:

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=event_manager
DB_USERNAME=seu_usuario
DB_PASSWORD=sua_senha
```

### 🔹 4️⃣ Gere a Chave da Aplicação  

```bash
php artisan key:generate
```

### 🔹 5️⃣ Execute as Migrations e Seeders  

Crie as tabelas no banco de dados e, opcionalmente, adicione dados iniciais:

```bash
php artisan migrate --seed
```

### 🔹 6️⃣ Inicie o Servidor  

```bash
php artisan serve
```

Agora, acesse no navegador:  
🔗 **[http://127.0.0.1:8000](http://127.0.0.1:8000)**

---

## 🔑 Credenciais Padrão (Se houver login)

Caso o projeto tenha autenticação de usuários, utilize as credenciais de teste:

- **Usuário:** `admin@example.com`
- **Senha:** `password`

---

## 📂 Estrutura do Projeto

O projeto segue a estrutura padrão do Laravel:

```
event-manager-laravel/
│── app/               # Lógica do backend (Controllers, Models)
│── bootstrap/         # Configuração inicial do Laravel
│── config/            # Arquivos de configuração
│── database/          # Migrations e Seeds
│── public/            # Arquivos públicos (CSS, JS, imagens)
│── resources/         # Views e assets do frontend
│── routes/            # Definição das rotas da aplicação
│── storage/           # Arquivos temporários, logs, cache
│── tests/             # Testes automatizados
│── .env               # Configuração do ambiente (NÃO SUBIR PARA O GIT)
│── artisan            # CLI do Laravel
│── composer.json      # Dependências do Laravel
│── package.json       # Dependências do frontend (Node.js)
│── README.md          # Documentação do projeto
```

---

## 💡 Dicas Extras

🔹 **Caso a porta `8000` esteja ocupada**, rode o servidor em outra porta:  
```bash
php artisan serve --port=8080
```

🔹 **Se precisar limpar o cache do Laravel**, execute:  
```bash
php artisan cache:clear
php artisan config:clear
php artisan route:clear
php artisan view:clear
```

🔹 **Erros de permissão no Linux?**  
Caso precise dar permissão às pastas de cache e logs:  
```bash
chmod -R 777 storage bootstrap/cache
```

---

## 🎯 Conclusão

Agora você tem tudo pronto para rodar o **Event Manager - Laravel** 🚀  
Caso tenha dúvidas ou precise de suporte, sinta-se à vontade para perguntar!  

🔥 **Divirta-se explorando e aprimorando o projeto!** 🎉

