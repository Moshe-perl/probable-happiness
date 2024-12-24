# probable-happiness

Project Description

This project demonstrates the use of SQL filters to enhance system security. The queries focus on investigating suspicious login activities and retrieving specific employee records for system updates. These examples are practical tools for organizations aiming to maintain a secure and well-managed IT environment.

Queries Overview

1. Retrieve After-Hours Failed Login Attempts
	•	Purpose: Identify failed login attempts that occurred after regular working hours (post 18:00).
	•	Details: Uses a success boolean column where 0 indicates a failure and 1 indicates a success. Filters for login attempts occurring after 18:00.

2. Retrieve Login Attempts on Specific Dates
	•	Purpose: Retrieve records of login attempts that happened on specific dates (e.g., 2022-05-08 and 2022-05-09).
	•	Details: Uses a string filter to match the exact dates provided.

3. Retrieve Login Attempts Outside of Mexico
	•	Purpose: Find login attempts originating from locations outside Mexico.
	•	Details:
	•	Uses the NOT operator to exclude records related to Mexico.
	•	Utilizes LIKE with the pattern MEX% to match entries starting with “MEX” (covering both abbreviations and the full name).

4. Retrieve Employees in Marketing
	•	Purpose: Find employees in the Marketing department who work in the East building.
	•	Details:
	•	Combines AND to ensure both conditions are met.
	•	Uses % as a wildcard to include office numbers followed by “East.”

5. Retrieve Employees in Finance or Sales
	•	Purpose: Retrieve all employees from either the Finance or Sales departments.
	•	Details: Uses the OR operator to include employees belonging to either department.

6. Retrieve All Employees Not in IT
	•	Purpose: Exclude records of employees in the IT department.
	•	Details: Applies the NOT operator to filter out entries where the department is IT.

Summary

These SQL queries leverage operators like AND, OR, and NOT, along with wildcard patterns, to:
	1.	Investigate suspicious login activities by analyzing timestamps, locations, and success rates.
	2.	Retrieve specific employee records to streamline security updates on relevant devices.

By applying these queries, organizations can ensure better data segmentation and proactive response to potential security threats.
