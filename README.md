# Projeto-Task-Manager
Projeto de verão com os colegas que visa criar uma aplicação para controlar equipas de trabalho em meio universitário e de trabalho

# Front-end
cd front-end
npm install
npm run dev

# Back-end
cd ../back-end
./gradlew bootRun

## Configuração da base de dados (back-end)
O back-end lê a ligação à base de dados das variáveis de ambiente `DB_URL`, `DB_USERNAME` e `DB_PASSWORD`.

- Opção 1: copiar `backend/.env.example` para `backend/.env` (ignorado pelo Git) e preencher os valores; o Spring carrega-o automaticamente ao correr `./gradlew bootRun` dentro de `backend/`.
- Opção 2: definir as variáveis no terminal (PowerShell: `$env:DB_URL = "jdbc:postgresql://<host>:5432/<db>"`, e o mesmo para `DB_USERNAME` e `DB_PASSWORD`; Bash: `export DB_URL=...`) ou na Run Configuration do IntelliJ (Environment variables).
