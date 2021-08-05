# Comandos Github | [Notas](../Readme.md)
- Iniciar Github `git init`
- Definir variable local Usuario `git config --global user.name "Levis-Code"`
- Definir variable local Correo `git config --global user.email "example@gmail.com"`
- `git add index.js`
- `git status`
- `git commit -m "Version 1.0"` 
- `git branch -M main`
- `git remote add origin git@github.com:Levis-Code/notes.git`
- `git push -u origin main`
>[Si da error de HASH](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
```
>ssh-keygen -t rsa -b 4096 -C “example@gmail.com”
>Generating public/private ed25519 key pair.
>Enter a file in which to save the key (/c/Users/you/.ssh/id_ed25519):[Press enter]```
> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]