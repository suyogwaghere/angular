# angualar
This is Assignment 3: C) Angular Application

** Commands To Execute In Terminal:
 1. npm --version     - It is used to check the version of nodejs 
 2. npm install @angular/cli@latest  - It is used to install angular cli
 3. ng new project_name      - It is used to create new angular project
 4. ng serve        - It is used to compile the code (Make sure you are in correct directory before executing this command)
 
 Then copy the localhost address with port and paste it in your browser (if it not redirected automatically to your default browser).


** Some Basic Questions That Can Be Asked:
 1. What is AngularJS?
 2. What are the features of AngularJS?
 3. Which commands have you used to implement this assignment? 
 4. Explain the code that you have written.

---
**NOTE**

HTML_file:
<h1> {{title}}</h1>
<input type="text" #name placeholder=":"enter your name" name="name"> </br>
<input type="text" #adress placeholder=":"enter your adress" name="adress"> </br>
<input type="text" #contact placeholder=":"enter your contact" name="contact"> </br>
<input type="text" #email placeholder=":"enter your email" name="email"> </br>
<input type="password" #password placeholder=":"enter your password" name="password"> </br>
<button (click)="getValue(name.value,adress.value,contact.value,email.value)" >Register</button>
<h1>Your Registered Data</h1><br>
<p> Name:{{dispalyname}}</p>
<p> Adress:{{dispalyadress}}</p>
<p> Contact:{{dispalycontact}}</p>
<p> Email:{{dispalyemail}}</p>

component.ts File:
under AppComponent
 dispalyname="";
  dispalyadress="";
  dispalycontact="";
  dispalyemail="";
  getValue(name:string,adress:string,contact:string,email:string){
this.displayname=name;
this.displayadresss=adress;
this.displaycontact=contact;
this.displaycontact=contact;
this.displayemail=email;
  }
                 
                 


It works with almost all markdown flavours (the below blank line matters).

---
