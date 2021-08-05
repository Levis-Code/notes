# Markdown | [Notas](../Readme.md)
## Librerias a instalar
* Instalar JSDoc `pnpm i jsdoc  -D`
*  Instalar plantillas `pnpm i clean-jsdoc-theme ink-docstrap tui-jsdoc-template`
*  Instalar plugin para documentar REST-API `pnpm i jsdoc-http-plugin` (agrega etiqueta @path, @header, @auth)
*  Instalar libreria para Deploy
`pnpm i gh-pages  -D`
 ## Comandos del package.json
 * Documentar: `pnpx jsdoc -c jsdoc.json` o crear script **package.json** `"doc": "jsdoc -c jsdoc.json"` 
 *  Deploy: `gh-pages -d doc` o crear script **package.json** `"doc-deploy": "gh-pages -d doc"` 

## Configuracion del jsdoc.json
```json
{
    "plugins":["jsdoc-http-plugin"],
    "source":{
        "include":["src"],
        "includePattern":".js$",
        "excludePattern":"(node_modules,docs)"
    },
    "templates":{
        "cleverLinks":false,
        "monospaceLinks":false
    },
    "opts":{
        "recurse":"true",
        "destination":"./doc",
        "template":"node_modules/ink-docstrap/template",
        "tutorials":"tutorials",
        "readme":"./Readme.md"
    }
}
```