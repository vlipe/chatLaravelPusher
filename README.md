# \# Chat Laravel — Comunicação em Tempo Real com WebSocket, Chatify e Pusher

# 

# Aplicativo web desenvolvido em Laravel para gerenciamento de comunicação síncrona e mensagens em tempo real.

# O sistema conta com autenticação de usuários gerenciada pelo \*\*Laravel Breeze\*\* e um painel completo de chat integrado via \*\*Chatify\*\*, utilizando a infraestrutura de WebSockets do \*\*Pusher\*\* para entrega instantânea de dados sem a necessidade de atualização de página.

# 

# \## Tecnologias e Arquitetura

# 

# \- \*\*Linguagem \& Framework Backend:\*\* PHP 8.x + Laravel 11

# \- \*\*Autenticação \& Sessão:\*\* Laravel Breeze (Blade / Alpine.js)

# \- \*\*Sistema de Chat:\*\* Chatify Package (`munafio/chatify`)

# \- \*\*WebSockets \& Protocolos:\*\* Pusher Channels (`pusher/pusher-php-server`)

# \- \*\*Banco de Dados:\*\* MySQL / MariaDB (via phpMyAdmin no XAMPP)\[cite: 1]

# \- \*\*Build Tool \& Bundler:\*\* Vite (`npm run dev`)\[cite: 1]

# 

# \## Funcionalidades da Aplicação

# 

# \- \*\*Autenticação de Usuários:\*\* Cadastro, login, logout e gerenciamento de perfil com validação do Laravel Breeze\[cite: 1].

# \- \*\*Chat em Tempo Real:\*\* Envio e recebimento instantâneo de mensagens com WebSocket via Pusher Channels\[cite: 1].

# \- \*\*Interface do Chatify:\*\*

# &nbsp; - Lista dinâmica de contatos e usuários cadastrados.

# &nbsp; - Indicadores de status de presença e mensagens enviadas/lidas.

# &nbsp; - Suporte ao envio de mídias e arquivos na conversa.

# &nbsp; - Design responsivo integrado ao ecossistema do Laravel.

# 

# \## Como Executar o Projeto

# 

# \### Pré-requisitos

# 

# \- \*\*XAMPP\*\* (com Apache e MySQL ativos)\[cite: 1]

# \- \*\*PHP\*\* (v8.2 ou superior)\[cite: 1]

# \- \*\*Composer\*\*\[cite: 1]

# \- \*\*Node.js\*\* e \*\*npm\*\*\[cite: 1]

# \- Conta ativa na plataforma \*\*Pusher Channels\*\*\[cite: 1]

# 

# \### Passo a Passo

# 

# 1\. \*\*Clone o repositório:\*\*

# &nbsp;  ```bash

# &nbsp;  git clone \[https://github.com/vlipe/chatLaravelPusher.git](https://github.com/vlipe/chatLaravelPusher.git)

# &nbsp;  cd chatLaravelPusher

