# angualar
This is Assignment 3: C) Angular Application

** Commands To Execute In Terminal:
 1. npm --version     - It is used to check the version of nodejs 
 2. npm install @angular/cli  - It is used to install angular cli
 3. ng new project_name      - It is used to create new angular project
 4. ng serve        - It is used to compile the code (Make sure you are in correct directory before executing this command)
 
 Then copy the localhost address with port and paste it in your browser (if it not redirected automatically to your default browser).


** Some Basic Questions That Can Be Asked:
 1. What is AngularJS?
 2. What are the features of AngularJS?
 3. Which commands have you used to implement this assignment? 
 4. Explain the code that you have written.
<p>
**NOTE**
`code here
<p> Name:{{dispalyname}}</p>
<p> Adress:{{dispalyadress}}</p>
<p> Contact:{{dispalycontact}}</p>
<p> Email:{{dispalyemail}}</p>
`


HTML_file:
<!-- Toolbar -->
<h1> {{title}}</h1>
<input style="margin: 5px 5px;" type="text" #name placeholder="Enter your name" name="name"><br>
<input style="margin: 5px 5px;" type="text" #adress placeholder="Enter your address" name="address"><br>
<input style="margin: 5px 5px;" type="text" #contact placeholder="Enter your contact" name="contact"><br>
<input style="margin: 5px 5px;" type="text" #email placeholder="Enter your email" name="email"> <br>
<input style="margin: 5px 5px;" type="password" #password placeholder="Enter your password" name="password"><br>
<button style="margin: 15px;" (click)="getValue(name.value,adress.value,contact.value,email.value)" >Register</button><br>
<h1>Your Registered Data</h1><br>
<p> Name:{{displayname}}</p>
<p> Address:{{displayaddress}}</p>
<p> Contact:{{dispalycontact}}</p>
<p> Email:{{displayemail}}</p>
<router-outlet></router-outlet>

component.ts File:
import { Component } from '@angular/core';
@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'Register Here  ';
  displayname="";
  displayaddress="";
  dispalycontact="";
  displayemail="";
  getValue(name:string,address:string,contact:string,email:string) {
      this.displayname=name;
      this.displayaddress=address;
      this.dispalycontact=contact;
      this.displayemail=email;
  }
}
  }</p>



