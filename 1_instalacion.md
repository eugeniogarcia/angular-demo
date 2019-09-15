# Installation
```
npm install -g @angular/cli
```  

```
ng new AccountOwnerClient
```  

n Angular version 7, as soon as we type this command, two questions will appear. The first one is whether we want our project to have routing created, and the second one is about what kind of styling we want in our project. We are going to answer NO (N) for the first question, and (CSS – just hit enter) for the second one.  

We are going to use the bootstrap library for the styling, so let’s install it with the command:  
```
npm install --save bootstrap@3
```

Actualiza `angular.json`:  
```
"styles": [
              "src/styles.css",
              "./node_modules/bootstrap/dist/css/bootstrap.min.css"
            ],
```

Instala:  
```
npm install --save @types/bootstrap
```

Actualiza `tsconfig.app.json`:  
```
  "compilerOptions": {
    "outDir": "./out-tsc/app",
    "types": ["bootstrap"]
  }
```

Instala:  
```
npm install --save jquery
npm install --save @types/jquery
```

Actualiza `angular.json`:  
```
"scripts": [
        "./node_modules/jquery/dist/jquery.min.js",
        "./node_modules/bootstrap/dist/js/bootstrap.min.js"
]
```

Actualiza `tsconfig.app.json`:  
```
"types": ["bootstrap",
            "jquery"]
```

Instala:  
```
npm install --save jqueryui
npm install --save @types/jqueryui
```

Actualiza `angular.json`:  
```
"styles": [
    "src/styles.css",
    "./node_modules/bootstrap/dist/css/bootstrap.min.css",
    "./node_modules/jqueryui/jquery-ui.min.css",
],
"scripts": [
    "./node_modules/jquery/dist/jquery.min.js",
    "./node_modules/bootstrap/dist/js/bootstrap.min.js",
    "./node_modules/jqueryui/jquery-ui.min.js"
]
```

# Creating a New Component