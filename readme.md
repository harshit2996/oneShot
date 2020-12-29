# Demo

<img src = "https://github.com/harshit2996/oneShot/blob/master/OneShot_Desktop_Mode_Harshit_Singh.gif" width="100%" contain/>

# Steps to Run the Project
1. Set Up a MongoDB Database.
2. Create and populate Collections using the respective json files, i.e, 'students.json' and 'colleges.json' for 'students' and 'colleges' collections respectively or populate using own data as per the defined schemas in the backend/models.
3. Run ```npm install``` in backend and frontend directories to install the dependencies.
4. Configure the ```.env``` files with the base urls, ports and MongoDB database configurations for both the backend and the frontend
5. Start the MongoDB Server
6. Run ```node index.js``` or ```nodemon index.js``` in backend to start the server 
7. Run ```npm start``` in Frontend to run the React.JS Application

## Features 

1. The Home Page displays the Distribution of Pecentage of Colleges in India per State from the Colleges Collection in the Database.
2. The Students Page Displays List of all the students in the students collection.
3. Colleges Page has a form which takes name of College as Input and Displays the Details of the College

### API Endpoints - 
1. ```GET '/getAllStudents'``` - Fetches all records from students collection.
2. ```GET '/collegesByStates'``` - returns array of Objects with Structure as ```[ { State : Number of Colleges in State } ]```.
3. ```POST '/collegesByStates'``` - Fetches all records from Colleges where Name of state is same as POST data.
4. ```POST '/college'``` - Enter or Create a new College record in the Database with POST data as Object with College Details.
5. ```POST '/student'``` - Enter or Create a new Student record in the Database with POST data as Object with Student Details.
6. ```POST '/getCollegeDetails'``` - Fetch Details of the College in the POST data.

### Pages - 
1.  ```'/'``` Home Page
2.  ```'/colleges'```Get College Details by entering College Name in Form
3. ```'/students'``` Get List of All Students, Click on a Stuent Name to get his Details like Skills , college_id, batch, etc.  


<img src = "https://github.com/harshit2996/oneShot/blob/master/OneShot_Responsive_Mode_Harshit_Singh.gif" width="100%" contain/>

#### Responsive Mode Demo

### Tech Stack 
-  Node.JS (Express)
-  React.JS
-  Tailwind.CSS
-  Semantic UI (for Components)
-  Reacharts (For Pie / Doughnut Chart) 