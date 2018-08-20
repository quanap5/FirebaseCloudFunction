# FirebaseCloudFunction
Using Firebase Cloud Function in Ionic application

# Instalation
The principle step for this project
- Create the functions locally
- Push them to FIrebase
- Use on ionic Ionic application

# Step by step for installing

- In ordor to communicate with Firebase, we need globally install Library
+ npm install -g firebase-tools

- Create our project with name ionic-firebase-cloud-function
+ ionic start ionic-firebase-cloud-functions

- This is result on your project

+ [img] 

- Play role as database we have to create Firebase project as here [Tutorial create Firebase project]
+ <img src="https://github.com/quanap5/FirebaseCloudFunction/blob/master/demo/createFirebaseProject.PNG">

- Login into Firebase account
+ firebase login
+ <img src="https://github.com/quanap5/FirebaseCloudFunction/blob/master/demo/firebase_login.PNG">

-Setting up Firebase at the root of the your project
+ firebase init functions
+ <img src="https://github.com/quanap5/FirebaseCloudFunction/blob/master/demo/firebase_init_functions.PNG">

-the firebaserc will contains the name of your Firebase project
+ <img>

-the functions folder contains:
+ the index.js file is the function will be deployed
+ the node3_modules folder is where containing the libraries suchas moment.js, loadsh, etc.
+ the packages.json is information about the project, libraries, etc.

# Now is for function creation
- function is implemented on index.js file (JS is for Javascript code, you can implement function on Typescript code)
+ https://firebase.google.com/docs/functions/get-started

-Deploy using the following command
+ firebase deploy --only functions

Note: Errors Error: functions predeploy error: Command terminated with non-zero exit code4294963238

Edit content in firebase.Json to "npm --prefix \"%RESOURCE_DIR%\" run lint"

- <img src="https://github.com/quanap5/FirebaseCloudFunction/blob/master/demo/deployfunction2.PNG">
- <img src="https://github.com/quanap5/FirebaseCloudFunction/blob/master/demo/deploySucess.PNG">





