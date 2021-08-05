# Ayuda sobre Github



- `git checkout SHA1_HASH` //retorna a un commit especifico
- `git checkout archivo.js` //retorna los cambios
- `git checkout login` //retorna a la version login

- `git diff archivo.js` //muestra los cambios

- `git branch` //muesta las versiones
- `git branch login` //crea la version login

- `git log` //muestra los commit
- `git log --decorate --oneline --all --graph` //muestra un log con decorado
- `git reflog` //muestra los commit sin importar donde estes

# Comandos para subir a github

- `git commit -m "first commit"`
- `git branch -M main`
- `git remote add origin https://github.com/Oslay92/jsdoc-studio.git`
- `git push -u origin main`

- `git stash` salva el estado actual


# Paquetes para documentacion y correcion de codigo

-  eslint eslint-config-airbnb-base eslint-config-prettier eslint-plugin-import eslint-plugin-prettier  prettier

# Script

- `"start": "node src/index.js"` Inicia aplicacion
- `"dev": "nodemon -r dotenv/config src/index.js --ignore ask.json"` Inicia servidor de desarrollo nodemon
- `"lint": "eslint src/"` Inicia ESlint
- `"lint-fix": "eslint src/ --fix"` Corrige errores de codigo
- `"doc": "jsdoc -c jsdoc.json"` Crea documentacion
- `"deploy-doc": "gh-pages -d doc"` Publica documentacion
- `"deploy-heroku": "git push heroku master"` Sube proyecto a Heroku
