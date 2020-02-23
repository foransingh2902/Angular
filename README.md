# Angular
Angular 4 Self Learning

npm install
(minimum node version required is v6.9 to run angular)
npm install -g @angular/cli
ng --version


ng new hello-world (creates a new angular project named hello world. Run the command in the directory of VS code and it will automatically
be loaded in VS code when project completion is finish)

Go inside the project folder created by the above command using cd hello-world and run
ng serve
here we used angular cli to load our application in a web server. ng serve automatically calls the transcript compiler under the hood.


By default the app will be up on
http://localhost:4200/
it will create a file for javascript - main.js and for CSS - styles.js


install the latest typescript version by using this command
npm install -g typescript


code main.ts  -> will create a transcript file named main.ts and open it in vscode
tsc main.ts  -> this will call the transcript complier and create a main.js file (We can open the main.js using cmd by typing - code main.js).
We can compile this javascript file using
node main.js
else we can combine both commands as tsc main.ts && node main.js


tsc --target ES6 main.ts (by default the target compiler is ES5, if you are using any ES6 function then it won't run on ES5 compiler)
after this run the code as usual- node main.js


run this one if the ng g c course command didn't allowed to be run in VS code terminal
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
ng g c course
g - generate, c - component. This will create a component named course. It will create a folder name course and inside it will add
four files 
CREATE src/app/course/course.component.html (21 bytes)
CREATE src/app/course/course.component.spec.ts (628 bytes) to write unit tests
CREATE src/app/course/course.component.ts (275 bytes)
CREATE src/app/course/course.component.css
the last thing it will do is 
UPDATE src/app/app.module.ts (609 bytes)
and register our component in app.module.ts


to create service type
ng g s email
g - generate, s - service. This will not create any foldera and will add 2 files to the src/app folder
CREATE src/app/email.service.spec.ts (352 bytes)
CREATE src/app/email.service.ts (134 bytes)  to write unit tests
