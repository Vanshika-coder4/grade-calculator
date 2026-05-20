Grade Calculator
A comprehensive command-line grade calculator written in Python.
Enter marks for multiple students, get instant grades with personalised comments, view class statistics, search by name, and save reports to file.

How to Run
python3 week2/grade_calculator.py

Features
Grade calculation — A / B / C / D / F based on average marks
Personalised comments — unique feedback message per grade
Multiple students — enter as many students as needed in one session
3 subjects per student — marks collected and averaged automatically
Formatted results table — aligned columns, color-coded grades
Class statistics — average, highest, lowest, grade distribution chart
Student search — find any student by partial name match
Save results — exports a .txt report and a .json data file
Menu system — navigate all features from a numbered menu
Input validation — every input is validated with clear error messages
Grading Scale
Grade	Mark Range	Comment
A	90 – 100	Outstanding!
B	80 – 89	Great job!
C	70 – 79	Satisfactory
D	60 – 69	Needs improvement
F	0 – 59	Did not pass
Menu Options
1. Enter student data        — collect names and marks
2. View results table        — formatted table with color grades
3. View class statistics     — avg, high, low, grade distribution
4. View individual comments  — personalised feedback per student
5. Search for a student      — partial name search
6. Save results to file      — saves .txt report + .json data file
7. Exit

Output Files
When you choose Save results (option 6), two files are created in week2/:

File	Contents
results_YYYYMMDD_HHMMSS.txt	Human-readable report with table, stats, and comments
results_YYYYMMDD_HHMMSS.json	Structured data for further processing
Python Concepts Used
Concept	Where applied
if / elif / else	get_grade() — grade band logic
for loop	Collecting data for each student
while loop	Input validation loops
try / except	Catching invalid numeric input
Lists	Storing all student result dictionaries
Functions	get_grade, get_comment, collect_students, calculate_statistics, etc.
File I/O	Saving .txt and .json reports
json module	Serialising results to JSON
datetime module	Timestamping saved files
ANSI color codes	Color-coded terminal output
Project Structure
week2/
├── grade_calculator.py   # Main program
├── README.md             # This file
└── results_*.txt / .json # Generated when you save results

