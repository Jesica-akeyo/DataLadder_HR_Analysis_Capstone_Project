# Salt Corporation HR Data Analysis

## The question behind the work

 This project is the capstone for the Data Ladder Data Analysis Mentorship program, working with an HR dataset built for a fictional company called Salt Corporation. The dataset held a thousand employee records collected between 2018 and 2020, across five departments and five roles, and the actual assignment was treating every one of those records with the scrutiny a real HR or finance team gives payroll and retention numbers.

## What I did

- Salary values had a mix of numbers and spelled-out amounts like "sixty thousand," alongside missing entries recorded as blank cells or "NAN" text, so I converted every text value into a number and filled the missing entries using the average salary for the matching department and position
- Age carried text entries like "thirty" alongside empty cells, so I rebuilt the entire column with a formula that calculates age directly from birth year, keeping the figure accurate as the reference year moves forward
- Department names carried mixed capitalization, "finance" sitting beside "FINANCE," so I standardized every entry into one consistent category using text functions and targeted logic for the codes that needed extra handling
- Joining dates had several formats at once, so I extracted the day, month, and year from each entry separately and rebuilt every date into one uniform format
- Missing email addresses got reconstructed directly from each employee's first name, last name, and the company's domain, giving every record a working, correctly formatted address
- Benefits enrollment came recorded as "Yes," "YES," "Y," "no," and blank cells, so I built a clean three-way column that separated a confirmed yes, a confirmed no, and a genuine unknown, since a blank cell carries a different meaning from an explicit no

With a clean sheet in place, I built pivot tables in two layers. The first laid out the descriptive picture, headcount, salary, age, tenure, training, and satisfaction, each cut by department and role. The second tested sharper questions: attrition patterns across every cut of the data, the link between satisfaction and attrition, whether benefits enrollment tracks with retention, and whether pay actually tracks performance. I turned the findings into a slide narrative and a dashboard, so the analysis could stand on its own for a reader who opens the deck first and the spreadsheet second.

## What I found

- Salt Corporation carries a 39.2% attrition rate, and that rate holds steady across every department, every role, every employment type, and every tenure band, pointing to a pattern that reaches every corner of the company at close to equal strength
- Job satisfaction shows the clearest link to attrition anywhere in the dataset: employees who left scored satisfaction at 2 out of 5 on average, employees who stayed scored 3 out of 5, and that gap holds steady across every department and role
- Pay levels sit essentially flat against performance, with an A-grade performer earning close to the same average salary as an F-grade performer, a signal that reward and merit have drifted apart from each other
- Benefits enrollment covers only 42.9% of the workforce, and enrolled and unenrolled employees leave at almost identical rates, suggesting the current package carries limited weight in someone's decision to stay
- Finance carries the largest headcount alongside the second-lowest average salary and the smallest training investment of any department, a combination that lines up closely with its attrition rate
- Training hours average 42 a year company-wide, and directors, the group most likely to shape team culture, receive the least of it at 40 hours, and clerks receive the most at 45

[Link to the workbook: https://github.com/Jesica-akeyo/DataLadder_HR_Analysis_Capstone_Project/blob/36c79c2112242433814115d75e910628a2e58241/HR_data%20Project%20Analysis.xlsx ]
[Link to the presentation deck: https://github.com/Jesica-akeyo/DataLadder_HR_Analysis_Capstone_Project/blob/05bedb5793eda53823f87f362aa815761ce35d3b/SALT%20CORPORATION%20HR%20ANALYSIS.pptx ]

## Why this connects to data integrity work

The cleaning step took longer than the analysis itself, and that ratio matches what real data work looks like once it leaves a classroom. Every average calculated later rested on a decision made earlier about how to read one messy cell, a spelled-out salary, a missing email, a blank benefits field, and keeping the raw sheet next to the cleaned one meant every number in the final deck could be traced back to the row it came from. That habit, tracing a summary figure to its source and treating a blank cell as its own category, separate from a confirmed no, carries into any analysis resting on data that other people will use to make decisions.

## Tools

Excel, structured tables and PivotTables, formula-based data cleaning, alongside SQL and Power BI as part of the same certificate programme.

## Where this goes next

I want to carry the same cleaned dataset into a Power BI dashboard next, giving the findings a form built for people to explore the numbers on their own terms, beyond a fixed set of slides.
