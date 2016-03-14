# Pixelmasher Portfolio App

Sails + Jade + Sass + Bootstrap

### Dependencies

- Postgresql: install database
- Postico: postgres gui

### Prerequisites

```bash
npm install sails -g
npm install -g foreman
```

### Setup

clone repo
```bash
git https://github.com/evolmk/pixelmasher.git
cd pixelmasher
```
update your own database settings
```bash
cp .env.example .env
```

install dependencies
```bash
npm install
```

create database
```bash
psql -h localhost
create database pixelmasher;
```

### Run

```bash
nf start
sails lift (without node foreman)
```

### Deploy to Heroku
create app
```bash
heroku create pixelmasher-app
```
add `Procfile` file to app's root
```
web: node app.js

```

deploy
```bash
git push heroku master
```
