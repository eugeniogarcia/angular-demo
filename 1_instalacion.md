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

It will install the library but we also need to import its path into the angular-cli.json (In Angular 6 it is angular.json) file. Place it right above the styles.css.  
