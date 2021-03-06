# Mateu-application-framework
This is Mateu's application framework. 

It consists of a serie of frameworks which, together, will allow you to easily build your bussiness application.

By using java inheritance and polymorfism, you can easily extend existing aplications (e.g.: extend an ERP to create vertical solutions lke a PMS or a CRS).

They are mainly for java users, though I plan to migrate this project to .Net.

## Map

Mateu's application framework is compund of:

- mateu-ui
- mateu-rpc
- mateu-mdd

### Mateu-ui
Mateu-ui is a technology agnostic user interface framework which allows you to write your code with high-level components, in a client-side technology agnostic way. 

It also allows to to debug/test locally using javafx and deploy to a web application.

You can choose to build client side or server side applications.

### Mateu-rpc
Mateu-rpc is a framework/library which allows you to easily create a client-server communication layer. 

Just define services interfaces and implement them in your server side code. Mateu-rpc will create the client-side asynchronous interfaces and clients, and will publish your server side code as needed.

### Mateu-mdd
Mateu-mdd is a light Model Driven Development (MDD) framework. 

It creates mateu-ui components (views, menu entries, ...) from your JPA annotated classes.

### Mateu-case
Mateu-case is a CASE tool.

It allows you to define your application without writing code.

Using a web interface you can define your model objects and your app components, and the application will be immediately available online.

I have to check costs and everything, but this will be useful for easily create little applications.

## Mateu's way of building apps
The best way to create your own mateu app is to use one of the provided maven archetypes and, from there, modify the code to build your own app.

You should first decide which type of application you want to create:

- ui only app
- database app

Anycase you will have to choose if you want to build a client-side or a server-side app.

If you want to build a client-side app and you want to communicate with server-side code then you will add the mateu-rpc framework to your project.

At last, if you want to generate your mateu-ui components from your SQL tables, JPA entities or java classes.


## Maven and Gradle
I extensively use Maven and Gradle in these projects to avoid writing plugins for eclipse, idea or whatever.

It provides me a neutral way of adding the extra point to my projects, like creating templates(archetypes) or adding actions like run, deploy etc in an ide agnostic way.


## Mateu .Net

Yes, I plan to create a .Net port of this framework.

The same principles, the same ideas but in .Net.

First I will finish the java side, though ;)
