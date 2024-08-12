# A Simple FireBase Connection and Data adding data to Database in FireBase

## To implement this 

### 1. clone this repository using the below command:

``` git clone "https://github.com/sonalisrisivani/Firebase_Db_connection" ```

### 2. Now, Go to Firebase Console and and Create a Project and name it (I named it Demo). 

### 3. In Project section -> Go to Settings in Project Overview -> Project Settings -> your apps -> web icon </> in bottom -> appname- (i gave demo) -> set firebase hosting -> register app -> Add firebase SDK -> Here im using js, so -> use script tag -> copy the firebase cnfig which is displayed 


``` <script type="module">
  // Import the functions you need from the SDKs you need
  import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.5/firebase-app.js";
  import { getAnalytics } from "https://www.gstatic.com/firebasejs/10.12.5/firebase-analytics.js";
  // TODO: Add SDKs for Firebase products that you want to use
  // https://firebase.google.com/docs/web/setup#available-libraries

  // Your web app's Firebase configuration
  // For Firebase JS SDK v7.20.0 and later, measurementId is optional
  const firebaseConfig = {
    apiKey: "AIzaSyBAKkq__h1yq14Fey8KBPj8SSPXZ-3t0h0",
    authDomain: "fir-26ab4.firebaseapp.com",
    projectId: "fir-26ab4",
    storageBucket: "fir-26ab4.appspot.com",
    messagingSenderId: "841459619381",
    appId: "1:841459619381:web:f22d2efd5f73b5ca44837c",
    measurementId: "G-1MWSDDM5MJ"
  };

  // Initialize Firebase
  const app = initializeApp(firebaseConfig);
  const analytics = getAnalytics(app);
</script> ```



### 4. Copy that snippet and paste in the html file 

### 5. After Creating project , Create Database -> Firebase project -> build -> Firestore database -> Create database -> Enter Location -> Test mode -> Next -> Done. 

### 6. Start collections -> Document ID -> auto generate -> You can create as many collections as you want(I created a collection called login) ->  set columns/attributes for each of the collections with their respective DataTypes (I made 2 fields in the login collection , user_name : String and password : String) 



## Features:

-** User Registration **: users can reg by providing username and pw,it checks if it is already existed and if it don't , data will be sent to database
-** User Login **: users can login with their registered credentials , we perform fetching operation from db and ceck , if details matches, then alert box will display that logged in successfully.
-** Firebase Integration **: uses firebase firestore for storing and validating user credentials


## Technologies Used:

- ** HTML **: Structure of the web page.
- ** CSS **: Styling the web page.
- ** JavaScript **: Handling form submissions and Firebase interactions.
- ** Firebase **: Used for database management and authentication.

## Database Format:

-** Project name **: demo
-** Collection name **: login
-** Fields and their Datatypes **: 
   1. user_name (String)
   2. password (String)
