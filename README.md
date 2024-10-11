
# Whaticket - BRDSoft

Esse sistema tem o objetivo de unificar e facilitar a logistica e gestão de atendimentos, com criação de chamados e registro das conversar.


## Requsitos minimos

Node JS v16+, MariaDB e NVM


NVM:
```bash
sudo apt install nvm
```
Node JS:
```bash
nvm install 16
```
```bash
nvm use 16
```
MariaDB:
```bash
sudo apt install mariadb-server
```
```bash
sudo mysql_secure_installation
```

# Dependencia
```bash
sudo apt-get install -y libxshmfence-dev libgbm-dev wget unzip fontconfig locales gconf-service libasound2 libatk1.0-0 libc6 libcairo2 libcups2 libdbus-1-3 libexpat1 libfontconfig1 libgcc1 libgconf-2-4 libgdk-pixbuf2.0-0 libglib2.0-0 libgtk-3-0 libnspr4 libpango-1.0-0 libpangocairo-1.0-0 libstdc++6 libx11-6 libx11-xcb1 libxcb1 libxcomposite1 libxcursor1 libxdamage1 libxext6 libxfixes3 libxi6 libxrandr2 libxrender1 libxss1 libxtst6 ca-certificates fonts-liberation libappindicator1 libnss3 lsb-release xdg-utils
```
# Instalação
Instale as dependencias do projeto

Clone o projeto:

```bash
git clone https://github.com/carlosgguilherme/whaticket-community.git
```
```bash
cd whaticket-community
```
```bash
cd backend
```

```bash
cp .env.example .env
nano .env
```

```bash
BACKEND_URL=http://localhost
FRONTEND_URL=https://localhost:3000
PROXY_PORT=8080
PORT=8080

DB_HOST=                  
DB_DIALECT=
DB_USER=
DB_PASS=
DB_NAME=

JWT_SECRET=3123123213123
JWT_REFRESH_SECRET=75756756756
```

```bash
npm install
npm run build
npx sequelize db:migrate
npx sequelize db:seed:all
```

```bash
npm start
```
Clonar o arquivo .env
```bash
nano .env
REACT_APP_BACKEND_URL = http://localhost:8080/
```
Iniciar o projeto
```bash
npm start
```

