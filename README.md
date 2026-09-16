# Chat Laravel — Comunicação em Tempo Real com WebSocket, Chatify e Pusher

Aplicativo web desenvolvido em Laravel para gerenciamento de comunicação síncrona e mensagens em tempo real[cite: 1].
O sistema conta com autenticação de usuários gerenciada pelo **Laravel Breeze** e um painel completo de chat integrado via **Chatify**, utilizando a infraestrutura de WebSockets do **Pusher** para entrega instantânea de dados sem a necessidade de atualização de página[cite: 1].

## Tecnologias e Arquitetura

- **Linguagem & Framework Backend:** PHP 8.x + Laravel 11[cite: 1]
- **Autenticação & Sessão:** Laravel Breeze (Blade / Alpine.js)[cite: 1]
- **Sistema de Chat:** Chatify Package (`munafio/chatify`)[cite: 1]
- **WebSockets & Protocolos:** Pusher Channels (`pusher/pusher-php-server`)[cite: 1]
- **Banco de Dados:** MySQL / MariaDB (via phpMyAdmin no XAMPP)[cite: 1]
- **Build Tool & Bundler:** Vite (`npm run dev`)[cite: 1]

## Funcionalidades da Aplicação

- **Autenticação de Usuários:** Cadastro, login, logout e gerenciamento de perfil com validação do Laravel Breeze[cite: 1].
- **Chat em Tempo Real:** Envio e recebimento instantâneo de mensagens com WebSocket via Pusher Channels[cite: 1].
- **Interface do Chatify:**
  - Lista dinâmica de contatos e usuários cadastrados.
  - Indicadores de status de presença e mensagens enviadas/lidas.
  - Suporte ao envio de mídias e arquivos na conversa.
  - Design responsivo integrado ao ecossistema do Laravel.

## Como Executar o Projeto

### Pré-requisitos

- **XAMPP** (com Apache e MySQL ativos)[cite: 1]
- **PHP** (v8.2 ou superior)[cite: 1]
- **Composer**[cite: 1]
- **Node.js** e **npm**[cite: 1]
- Conta ativa na plataforma **Pusher Channels**[cite: 1]

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/vlipe/chatLaravelPusher.git](https://github.com/vlipe/chatLaravelPusher.git)
   cd chatLaravelPusher

```

2. **Instale as dependências do PHP e do Node.js:**
```bash
composer install
npm install

```


3. **Configure o Banco de Dados:**
* Crie uma base de dados no phpMyAdmin chamada `chatweb3ams`.




4. **Configuração de Variáveis de Ambiente (`.env`):**
* Renomeie ou copie o arquivo `.env.example` para `.env`:
```bash
cp .env.example .env

```


* Gere a chave da aplicação:
```bash
php artisan key:generate

```


* Atualize as configurações do banco de dados e do Pusher no arquivo `.env`:


```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=chatweb3ams
DB_USERNAME=root
DB_PASSWORD=

BROADCAST_DRIVER=pusher

PUSHER_APP_ID=seu_app_id
PUSHER_APP_KEY=sua_app_key
PUSHER_APP_SECRET=seu_app_secret
PUSHER_HOST=
PUSHER_PORT=443
PUSHER_SCHEME=https
PUSHER_APP_CLUSTER=us2

```




5. **Execute as Migrações da Base de Dados:**
```bash
php artisan migrate

```


6. **Execute a Aplicação:**
* Em um terminal, inicie a compilação dos assets:


```bash
npm run dev

```


* Em outro terminal, inicie o servidor do Laravel:


```bash
php artisan serve

```




7. **Acesse no Navegador:**
* Acesse `http://127.0.0.1:8000` para realizar o cadastro e login de usuários.


* Acesse `http://127.0.0.1:8000/chatify` para utilizar a interface do chat em tempo real.





```

```
