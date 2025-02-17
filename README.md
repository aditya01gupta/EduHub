1. Database Setup (setup_database())
When the program starts, it checks if the study_log.db database exists.
If not, it creates a study_log table to store study records.

2. Main Menu (main()) 
Displays options:
1. Log Study Session
2. Analyze Performance
3. Suggest Study Schedule 
4. Exit
Waits for the user’s choice and calls the corresponding function.

3. Logging a Study Session (track_study())
Prompts the user for subject, topic, time spent, difficulty, and score.
Stores the data in the SQLite database with the current date and time.

4. Analyzing Performance (analyze_performance())
•	Retrieves all study records from the database.
•	Calculates and displays the average score for each subject

5. Suggesting a Study Schedule (suggest_study_schedule())
•	Retrieves time spent and scores from the database.
•	Uses Linear Regression to predict the expected score if the user studies for 90 minutes.
•	If no data is available, it informs the user.

6. Checking for a milestone (check_badges())
•	The Beginner, Intermediate, Advanced or mastermind badges.
•	Motivate the user to strive for more points and thus, work harder.

7. Updating the study session (add_study_session())
•	Fetches the study session from the database.
•	Displays the entire past activity of the user. 

6. Program Loop & Exit
•	The menu repeats until the user chooses Exit (5).
•	If an invalid choice is entered, the program asks for a valid option.

