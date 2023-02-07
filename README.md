# Pewlett-Hackard Analysis - Module 7 Challenge
<sub>Chapel Hill - Data Science Bootcamp</sub>

## Overview of Project
For Module 7, data from Pewlett-Hackard's employees was given to be analyzed in preparation for the upcoming "silver tsunami," or the mass retiring of a generation. With information on the departments, department employees, department managers, employees, salaries, and titles, four CSV files were created to highlight the staff members who are likely to retire soon, their titles, and the staff members eligible to mentor others to replace them.

## Results
### Deliverable 1 - The Number of Retiring Employees by Title
- Retirement Titles
    - This table was created to list all employees born between 1952 and 1955, which would put their age in the range of the current "silver tsunami." By joining the [employees] and [titles] tables, the [retirement_titles] table contains each affected employee's ID number, first and last name, title, the date they were hired, and the date they left the company (if the employee is still hired, this date is "9999-01-01").
    - ![Retirement titles table](/Resources/retirement_titles.png)
- Unique Titles
    - Building off the previous table, the [unique_titles] table created a more concise list of soon-to-retire employees and their titles. The employees added to this table are still currently employed by the company, and are only listed once, with the title they currently hold.
    - ![Unique titles table](/Resources/unique_titles.png)
- Retiring Titles
    - Using [unique_titles], the [retiring_titles] table shows the number of employees per title who are likely to retire soon.
    - ![Retiring titles table](/Resources/retiring_titles.png)
- From these tables, it is evident that a large portion of employees are likely to retire in the upcoming "silver tsumani," with the vast majority of them (50,842 of a total 71,458 employees) being either a "Senior Engineer" or "Senior Staff." With a total of 300,024 employees, these staff members make up approximately 24% of the entire Pewlett-Hackard workforce. 
- After breaking the employees into groups based on their titles, the effects the "silver tsunami" will have become increasingly apparent. Below are two charts, one with the number of employees who are about to retire in each title, and another with the total number of employees for each title. Using these, we can calculate the percent of each department that are likely to retire, shown in the third figure.
- ![Number of employees to retire per title](/Resources/retiring_titles.png) ![Total number of employees per title](/Resources/all_titles_count.png)
- ![Percent of employees retiring per title](/Resources/titles_percent_retiring.png)
- As becomes evident from these figures, the role of "Senior Engineer" will likely suffer the loss of more than 85% of its employees, and Pewlett-Hackard will have to train and/or hire many people to fill these positions.

### Deliverable 2 - The Employees Eligible for the Mentorship Program
- Mentorship Eligibility
    - The [employees], [dept_emp], and [titles] tables were joined to show employees born in the year of 1965 who are still working with the company and the titles they currently show.
    - ![Retirement titles table](/Resources/retirement_titles.png)
- In the resulting table, 1,549 staff members fit the eligibility requirements for becoming a mentor to younger employees. After breaking them down into groups of their titles, it becomes clear that there are not enough mentors to help fill the spots left by retiring employees.
- ![Number of mentors per title](/Resources/mentorship_eligibility_count.png) ![Percent of mentors versus retiring employees](/Resources/titles_percent_mentors.png)
- Again, "Senior Engineers" will face difficulties in training enough employees to fill the empty positions with 25,916 employees leaving and only 241 mentors to train new members.

## Summary
- As the "silver tsunami" begins to make an impact, a total of 72,458 employees at Pewlett-Hackard are likely to retire. Of these, 25,916 are "Senior Engineers" and 24,926 are "Senior Staff," which will require many new hires and an abundance of training.
- Based on the current requirements for becoming a mentor, there are not enough Pewlett-Hackard employees eligible to mentor the next generation of the company's workforce. There are a total of 1,549 employees currently eligible to become mentors; compared to the 72,458 employees about to retire, the ratio of mentors to retirees is roughly 1:47, or 2.1%. However, there are so few mentors because the requirements dictate that they are only allowed to be born in the year of 1965; if the company were to increase the age range, the number of eligible mentors would increase.
- The titles with the highest percentage of workers retiring are "Technique Leader," "Senior Staff," and "Senior Engineer," with rates of 23.8%, 26.8%, and 86.3%, respectively. With a total rate of 24.2% of the company retiring with the "silver tsunami," the number of "Technique Leaders" and "Senior Staff" are logical, but 86.3% of "Senior Engineers" is disproportionally large. In the future, it may benefit Pewlett-Hackard to conduct a quarterly/annual review of the number of employees in each role and monitor the percentage of workers in each age group. If large disparities are found like the current distribution of "Senior Engineers," they can be corrected over the next round(s) of promotions and hiring cycles.
- In line with the previous suggestion, Pewlett-Hackard would likely also benefit from consistently managing their overall workforce's age. Out of 300,024 total employees, 72,458 or 24.2% are born in the four-year range of 1952 to 1955. Looking at the list of all employees, the youngest was born in February of 1965, and the oldest in February of 1952. The company would see greatly increased longevity if they used the opportunity of the current "silver tsunami" to hire younger workers and lower the average age of their workers.
