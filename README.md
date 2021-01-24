# pandas_challenge

### contains:
* PyCitySchools.ipynb
* schools_analysis.pdf

### description:

The goal of this analysis was to uncover trends within the reading and mathematics yearly test scores from schools within a district in order to produce potential recommendations for budget allocations in future years.

The jupyter notebook PyCitySchools.ipynb therefore contains the following steps to reveal trends:
* Data Cleaning:
    * reading in two csvs as dataframes, one containing data on schools, the other containing student data (school_data, student_data respectively)
    * left merge the two dataframes in order to have data only on students connected to schools (schools_and_students_df)
* District-level summary:
    - number of schools: creating and finding the length of a list of schools (num_schools)
    - total number of students: finding the length of the 'Student ID' column(which contains unique values) in schools_and_students_df (num_students)
    - total budget: creating and finding the sum of a list of budgets (total_budget)
    - average mathematics exam score: finding the average of the math_scores column in schools_and_students_df (avg_maths)
    - average reading exam score: finding the average of the reading_scores column in schools_and_students_df (avg_reading)
    - percentage of students passing the mathematics exam: 
        - finding the length of the results of a boolean mask filtering for mathematics scores greater than or equal to 70 (students_passing_maths)
        - dividing the number of students passing by the number of students(students_passing_maths/num_students), multiplied times 100 to get a number of out 100.
    - percentage of students passing the reading exam: follows the same format as finding the percentage of students passing mathematics, with a boolean mask filtering for scores of 70 and above in reading (students_passing_reading) divided by total number of students
    - percentage of students passing both exams: follows a similar format as above, with a boolean mask filtering for scores 70 and above for both subjects (students_passing_both), divided by total number of students
    - creating the dataframe for display:
        - creating a dictionary of lists to hold the different values (summary_dict)
        - creating a dataframe out of the dictionary (district_summary_df)
        - creating a copy of district_summary_df to apply formatting in order to preserve district_summary_df for potential later use (district_summary_df_F)
            - once the formatting is applied, all the values will be strings, as opposed to numbers, which can no longer be used for mathematical operations
        - applying formatting to district_summary_df_F, and displaying it
* School level analysis:    
    * School-level summary:
    * Schools with top overall passing scores:
    * Schools with bottom overall passing scores:
    * Mathematics scores by grade:
    * Reading scores by grade:
    * School performance in exams based on school spending ranges:
    * School scores based on school type:
    * School scores based on school type:


