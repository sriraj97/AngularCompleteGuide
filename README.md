#  Angular Complete guide notes

## 2) What is Angular?
Angular => JS framework allows us to create  => reactive SPA’s
Page refersh wil not happen in browser  

## 4) Angular versioning?
Angular1(Angular JS)=>after flaw corrected Angular 2 rewritten in 2016 => Angular 3 skipped for some internal reasons => Angular 4 …. Angular 10,11,12…. 13,14,15 and so on
Angular is backward compatible

## 6) Project setup
Node js  server side language ,we don’t use node js codes but it is used behind by angular/cli
Npm  Node package manager to handle node package dependencies

### Commands :
#### npm install -g @angular/cli[@latest]
Go to our root folder using (cd)  ng new [appname] –no-strict {--no-strict  non-strict mode}
Then go to ur newly created project folder  cd my-first-app  ng serve 

### Angular uses ts, as super set of js

## 7) Editing First App:
There is IDE – WEBSTORM  for angular development but its not free
Command : go to app base folder and open cmd prompt  code .   opens project in VS Code
Dynamic data binding ,index.html,[(ngModel)]I\O Directive Binding to use this we need to add (FormsModule)   to the corresponding module.ts

## 8) Course Structure:
  Image is given in  **Angular Complete guide notes.docx**
 
## 10) what is TypeScript?
TypeScript is just Super Script of JavaScript. It offers more feature like classes,interfaces and also which has names,types, strong typing (no,string and Boolean).

Finally TS is complied to JS
*****npm install --save bootstrap@3*****

## SECTION -2 THE BASICS

## 15) How Angular App started and loaded?
Index .html  main html file with <html></html>  and also we can see <app-root></app-root> where angular app itself creates one component for us.
	In app.component.ts  we able to see @Component decorator   selector through which we connect all component related files(html,css & where to bind the corresponding functionality)
While viewing source code we can see couple of scripts imported like inline.bundle.js,polyfills.bundle.js ,etc.., injected by cli automatically 
	In Main.ts  platformBrowserDynamic().bootstrapModule(AppModule)  the place where app.module.ts is defined
	In app.module.ts  @NgModule { bootstrap :[AppComponent]  will get connected at the run time
	Angular in the end is JS framework changing your DOM (‘HTML’) at runtime
 
## 16) Components are important?
	Each Components has own business logic and more importantly each components is reusable
	bcaz we don’t need to write html ,css , js entirely in 1 corresponding files but split it up into n files 

## 17) New Component
	Decorator is used to enhance the elements

## 23) Component selector
	Selectors  can be used in general ways , like data attributes used in html  [app-server],like class in html  .app-server but we can’t use id attribute as selector

## 25) Data Binding
	Data Binding Communication b/w .ts and .html
	**	1&2  output data, 3  input data ,4	 2 way data
1. string interpolation {{data}} 
2. Property binding [prop]=”data”
3. event binding (event)=”expression”  input
4.  2 way binding [(ngModel)]=”data”**

## 26) string interpolation
	Any expression can resulted to string in the end
		**cant write multi line expressions ,
		Cant write block expressions,
		Cant write if, for control structure 
		We could use ternary expression
		We can even call a method in string interpolation	**
  
## 28) string interpolation vs property binding
	In simple string interpolation can be done using  property binding
For ex:
	**<p [innerText]="allowNewServer"></p>**









