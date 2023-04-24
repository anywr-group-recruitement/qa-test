[French version](README_FR.md)

# Welcome to Anywr Software Tester exam!
Before you begin, please read the following instructions carefully:

- This exam is designed to evaluate your knowledge and skills in various aspects of software testing, such as manual testing, test automation, database testing, API testing, and test planning.
- Please read each question carefully and provide clear, concise, and well-organized answers.
- Although we encourage you to complete all the topics in the exam, we understand that you may not have expertise in every area. If you are unable to complete a task or
answer a question, please do not worry. It is more important to showcase your strengths and provide thoughtful answers in the areas you are most comfortable with.

### Manual Testing

As a QA Tester, you are tasked with manually testing for freelance mission pages. The
application allows users to search for a mission and apply.

URL: <https://www.anywr.frl/en/freelance/freelance-mission>

**Task:**

- List the test cases you can draft for the search mission section
- Mention the Positive & Negative Scenarios. Organize the list of test cases by priority.
- Suggest enhancements that could improve the user experience or functionality. (If Exists)
- Identify and report any discovered bugs, if present

### API Testing - "Create Booking" Endpoint Validation"

As a QA Tester, you are tasked with testing the Restful Booker API, a simple RESTful API that
allows users to manage hotel bookings. Your primary focus is on the "Create Booking" endpoint,
which allows users to create new bookings.

Use the following link for the API Booking method:

<https://restful-booker.herokuapp.com/apidoc/index.html#api-Booking-CreateBooking>

- Set up the Restful Booker API in a popular API testing tool (e.g., Postman, Insomnia, or any other tool of your choice).
- Test the "Create Booking" endpoint with various test cases, covering positive, negative, and boundary scenarios.
- Identify and list any bugs or issues found during the testing process. Provide a brief description of each bug, including the test case, steps to reproduce, expected outcome, and actual outcome.

### Database Testing - User Registration and Login Validation

#### Exam 1

You are working on a web application that uses a relational database to store user information.
The application allows users to register and log in.

The following table holds user data:

```
User Table
- Id (INT, primary key, auto-increment)
- Email (VARCHAR, unique)
- Password (VARCHAR)
```

***Write SQL queries to test the following scenarios:***

- Add a new user to the User table.
- Verify that the new user is added to the Users table with the correct email and password after registration.
- Verify that a user cannot be added with an email that already exists in the Users table.



#### Exam 2

You have three tables (Customers, Orders and Employees) as below:

**Customers:**

| customer_id | customer_name  | customer_email          |
|-------------|----------------|-------------------------|
| 1           | John Doe       | john.doe@mail.com       |
| 2           | Jane Smith     | jane.smith@mail.com     |
| 3           | Bob Johnson    | bob.johnson@mail.com    |
| 4           | Sarah Williams | sarah.williams@mail.com |
| 5           | Diana smith    | Diana.smith@mail.com    |
| 6           | Will storm     | Will.storm@mail.com     |

**Orders:**

| order_id | customer_id | order_date | order_amount |
|----------|-------------|------------|--------------|
| 1        | 1           | 2022-04-16 | 100.00       |
| 2        | 1           | 2022-04-15 | 50.00        |
| 3        | 2           | 2022-04-14 | 75.00        |
| 4        | 3           | 2022-04-13 | 200.00       |
| 5        | 4           | 2022-04-12 | 150.00       |
| 6        | 6           | 2022-04-12 | 175.00       |
| 7        | 1           | 2022-01-12 | 120.60       |



**Employee:**

| employee_id | employee_name  | department_name | salary |
|-------------|----------------|-----------------|--------|
| 1           | John Smith     | Sales           | 50000  |
| 2           | Jane Doe       | Marketing       | 55000  |
| 3           | Bob Johnson    | Sales           | 60000  |
| 4           | Sarah Williams | Marketing       | 65000  |
| 5           | James Lee      | Finance         | 70000  |

***Questions:***

- Write a query to find the top 4 customers who have made the highest total purchase amount in the past month.
- Write a query to join two tables, "Customers" and "Orders", and return the names of all customers who have made an order in the past year.
- Write a query to calculate the average salary of employees in each department, and return the results sorted in descending order by average salary.

### Coding Questions:

**Multiple options questions:**

1 - Considering the below code , choose the correct output:
  - var a = “5”;
  - var b = “5”;
  - var sum = a+b;
  - console.log(sum);

**output :**
- “a+b”
- 10
- “55”


2 - Which method would you use to convert a string to all uppercase letters?
    - toLowerCase()
  - toUpperCase()
  - capitalize()
  - upper()


3 - Considering the below code, choose the correct output:

- var x = [1, 2, 3];
- console.log(x.length);

**output :**
- 0
- 1
- 2
- 3

### Automation Testing:

#### Section1: Multiple options questions:

1- You need to test a field accepting only numbers between 2 and 1000, each test case can verify using only one number.
  - Test 1 with the number (-1).
  - Test 2 with the number (1).
  - Test3 with the number (500).

**Which of the below responses is correct:**
- The test case 1 is a negative test case, the test cases 2 and 3 are positives.
- All test cases are positives.
- The test cases 1 and 2 are negative test cases, the test 3 in a positive test.
- All test cases are negatives.

2- What is an assertion in UI automation testing?

   - To confirm a previous test result
   - Report of test results
   - Summary of test steps
   - Summary of test case results

3- What is regression testing in UI automation testing?

   - Testing a new feature in isolation from the rest of the application.
   - Testing the same set of test cases repeatedly to ensure that no new bugs have been introduced.
   - Testing the application under different network conditions.
   - Testing the application under different browser.

## Section 2:

As a QA Tester, you are tasked with automating a UI test for the "Forgot Password" functionality
on the Talent Anywr Group login page. The application allows users to reset their passwords by
providing their email address.

URL: <https://talent.anywr-group.com/en/login>

- Choose your preferred automation tool (e.g., Selenium WebDriver, Cypress, TestCafe) and create a test script to automate the following test case:
   - Verify that the "Forgot Password" functionality sends a password reset email to the user's registered email address. (Note: ignore testing the email)
- Report any bugs found during the testing process. (If exists)
- Suggest enhancements to the "Forgot Password" functionality that could improve the user experience or functionality. (If Exists)

***If you possess experience in the areas of Performance, Load , StressTesting, or Security
Testing, could you please provide details about your relevant projects, accomplishments,
and expertise in these domains?***

**Best of Luck!**
