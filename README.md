# Angular
---

## Screenshots

### Tela principal

![Tela principal](/frontend/src/assets/img/principal.png "Tela principal")

---

## Backend

### Setup inicial

Executar:

```bash
npm init -y
npm i json-server
```

Incluir o script:

```json
"scripts": {
    "start": "json-server --watch db.json --port 3001"
  }
```

### Inicializar o serviço
Dentro da pasta do backend, executar:
```bash
npm start
```
---

## Frontend

### Setup inicial
```bash
sudo npm i -g @angular/cli
ng new frontend --minimal
```
Would you like to add Angular routing? y
Which stylesheet format would you like to use? CSS

Modificar o angular.json
```json
"@schematics/angular:component": {
  "inlineTemplate": false,
  "inlineStyle": false,
  "skipTests": true
}
```
Modificar o /src/app/app.component.ts

```bash
@Component({
  selector: 'app-root',
  templateUrl:'app.component.html'
})
```
Criar o template HTML do componente principal:
`/src/app/app.component.html`

Instalar o Material Design:

```bash
ng add @angular/material
```

### Inicializar o serviço de build do front
```bash
npm start
```

### Geração de componentes

Pode ser utilizado o comando `ng generate component <diretorio/nome-do-componente>` mas também pode ser abreviado para `ng g c`, conforme abaixo:

```bash
ng g c components/template/header
ng g c components/template/footer
ng g c components/template/nav
ng g c views/home
ng g c views/product-crud
ng g c components/product/product-read
ng g c components/product/product-create
ng g c components/product/product-update
```

### Geração de componentes do Material Design com esquemas

Pode ser utilizado o comando `ng generate @angular/material:<tipo-do-componente> <diretorio/nome-do-componente>`, conforme abaixo:

```bash
ng generate @angular/material:table components/product/product-read2
```

### Geração de diretivas

Pode ser utilizado o comando `ng generate directive <diretorio/nome-da-diretiva>` mas também pode ser abreviado, conforme abaixo:

```bash
ng g d directives/red
ng g d directives/for
``` 

### Geração de services

Pode ser utilizado o comando `ng generate service <diretorio/nome-do-serviço>` mas também pode ser abreviado, conforme abaixo:

```bash
ng g s components/product/product
``` 


## Plugin VS Code

[steoates.autoimport](https://marketplace.visualstudio.com/items?itemName=steoates.autoimport)
[johnpapa.angular2](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2)