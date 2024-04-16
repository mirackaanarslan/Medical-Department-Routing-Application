# Medical Department Routing Application
This application facilitates patients by directing them to the most appropriate medical department based on their entered personal information and reported symptoms. 

Additionally, serving as a decision support system, it aims to lighten the workload of healthcare professionals.

In this program, a scoring algorithm is used where personal information and answered questions assign various points to specific departments.
# First Stage: Collection of Patient Personal Information and Reported Symptoms
First, the patient fills out the personal information section on the form displayed on the screen. 

Then, the patient either uses the search box or manually selects the symptoms they are experiencing. 

These gathered details are then sent from the frontend to the backend using the POST method, and the backend stores this data in the database.


Personal Information -->

Age Range (years): 0-10, 10-20, 20-40, 40-60, 60+

Sex

Alcohol Use

Tobacco Use

Existing Medical Conditions: Allergy, Hypertension, Diabetes, Heart Disease

# Second Stage: Answering Relevant Questions
Using the GET method, the frontend requests data from the backend, which retrieves the patient's personal information and all questions from the database. 

Then, by matching the symptoms in the personal information with the questions, only the relevant questions for the selected symptoms are sent to the frontend. 

Once the relevant questions are listed on the screen and answered, the frontend uses the POST method to send the selected answers to the backend. 

The backend then records this data in the database.

# Third Stage: Department Routing
Using the GET method, the frontend requests data from the backend, which retrieves the patient's personal information and answered questions from the database. 

Employing a scoring algorithm, the backend assigns various points to specific departments based on the personal information and the answers to the questions. 

Subsequently, the backend sends the department with the highest score and its corresponding score to the frontend. 

The relevant department and its score are then displayed on the screen.


# Languages and Technologies

React (JavaScript library for creating dynamically updating content)

.NET 8.0 (Server-side application development framework)

PostgreSQL (SQL-based relational database management system)
