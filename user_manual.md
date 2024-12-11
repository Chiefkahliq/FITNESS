# User Manual
## Registering an Account
1. Go to the registration page by clicking on 'Register'.
2. Enter your desired username and password.
3. Click the 'Register' button to create your account.

## Logging In
1. Once registered, go to the login page.
2. Enter your username and password.
3. Click 'Log In' to access your dashboard, where you will receive a workout and diet plan.

## Logging Out
1. Click the 'Logout' link to safely log out of your account.
2. update 12/10/2024
3. Prototype User Manual (No Screenshots)
Introduction
The Fitness App is a simple prototype that allows users to register, log in, and access basic fitness-related resources. This initial version focuses on user authentication and presenting three sets of fitness-related information: workout plans, diet options, and meal plans.

System Requirements
A computer running Windows, macOS, or Linux.
Python 3.7 or higher installed.
A web browser (e.g., Chrome, Firefox).
Dependencies listed in the requirements.txt file (Flask, Flask-SQLAlchemy, Flask-WTF).
Installation Instructions
Clone the Repository:
Use git clone https://github.com/YourUsername/YourRepositoryName.git to clone the project locally, or download and extract the project files into a folder called fitness_app.

Set Up a Virtual Environment (Optional):

bash
Copy code
python3 -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
Install Dependencies:
From the fitness_app directory, run:

bash
Copy code
pip install -r requirements.txt
Initialize the Database:
Run a Python shell:

bash
Copy code
python
Then inside Python:

python
Copy code
from app import db
db.create_all()
exit()
Run the Application:

bash
Copy code
python app.py
Open a web browser and go to http://127.0.0.1:5000/.

Using the Application Features
Registering a New Account
Navigate to the /register route in your browser.
Enter a username and a password (password at least 8 characters).
Click the “Register” button.
You will be redirected to the login page after successful registration.
Logging In
Go to the /login page.
Enter your username and password.
Click the “Login” button.
You will be taken to the dashboard if your credentials are valid.
Viewing Workout Plans
After logging in, access the dashboard page.
You will see three basic workout plans (e.g., a cardio routine, a strength training routine, and a flexibility routine).
Viewing Diet Options
On the same dashboard, you can review three diet options (e.g., Low Carb, Mediterranean, High Protein).
Each option provides a brief description.
Viewing Meal Plans
Below the diet options, you’ll see three meal plans (e.g., recommended breakfast, lunch, and dinner options).
These are simple suggestions to help guide your daily eating habits.
Troubleshooting
If you cannot register, make sure the username is unique and meets any input requirements.
If you cannot log in, check that your username and password are correct.
If the dashboard data does not appear, ensure that the database was created correctly (db.create_all() was run) and that the app is running without errors.
Future Enhancements
Adding password reset functionality.
Tracking user-specific progress.
Integrating more detailed nutritional data and personalized workout recommendations.
