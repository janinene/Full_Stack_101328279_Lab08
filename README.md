# Lab08_101328279
Full Stack II  04-09-2023

Exercise #1 – Angular Component
1.	Create a folder named Lab08_StudentID
2.	Open a command prompt create a directory for exercise-1
3.	Open Visual Studio Code and open the folder exercise-1
4.	 Create a new project and default application named student-app by running the following Angular CLI command.
        ```ng new student-app```

5.	In the project structure, navigate to the source foleder (src) and then to the app folder.  Right click and add a new file named **students.component.ts**

6.	Create basic TypeScript class named StudentsComponent using Pascal casing, where every word starts with a capital letter.
    ```
    export class StudentsComponent {
    }
     ```
 
7.	Import the Component decorator from angular core.
 ```import {Component} from '@angular/core'```
 
8.	Add the Component metadata to make the class an Angular Component.
 ```
 @Component( {
    selector: 'students',
    template: '<h2>Students</h2>'
})
```

9.	Next we need to register this component in App module. Navigate to app.module.ts
in app folder.
 

10.	In the app.module.ts modify the NgModule decorator section to register the StudentComponent..
 

Type the name of the StudentComponent and press TAB, the import statement should auto-populate at the top of the page.

 


11.	Navigate to the app.component.html file. Open the file and delete all of the existing HTML markup in the page.
 
12.	Type following HTML code with out student selector <students></students>
 
13.	Use the Angular CLI to run the ng serve command to compile and load the application on localhost.
 
14.	Navigate to localhost:4200 to view the component in browser.

 

Exercise #2 – Creating Component with Angular CLI 

1.	Continue to work the same application in exercise-1 folder.
2.	Use the following Angular CLI command to generate a Component named student
 




The following boiler plate code files will be created for the Student component.
 

3.	Navigate to the new Student folder and review the generated StudentComponent.ts file.
 

Exercise #3 – Component Templates and First Binding

1.	Continue to work the same application in exercise-1 folder.
2.	Navigate back to our original Component file StudentsComponent.ts
3.	Add a field in the StudentComponent class named title.
 
4.	Update the Component Decorator to include a dynamic expression to update the view with the title.
 




5.	Add a method named getTitle() to the Component as follows
 
6.	Modify the Component Decorator to call function in the binding of the Template title
 

7.	Create a new method named getCurrentDate() that return the current date in the StudentComponent. 

8.	Update the Template Title to also display the Current Date from getCurrentDate(). Use the ES2015 Template Literal syntax in the string html.
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals
