# Open Cart Automation Testing

.)eCommerce Store is an ecommerce software Online Shopping Application, It organizes Online Shopping business operations like product promotions, selling products, and shipping goods etc. 
  It has two interfaces, One is Admin interface, provides features like Adding / Editing / Deleting Customers, Vendors, Products, User management and generating Reports. 
  Another interface is User Interface, provides features like User registration, Search products, Products Display, add to shopping cart, payments for Products and Buying products etc.

## Project contribution

 - [Ashrith]()
 - [Rajashekhar]()
 - [Chandu Taticonda]()

## Projects Technologies Used

1.  HTML (Hypertext Markup Language)               
2. CSS  (Cascading Style Sheets)         
3. JavaScript                                                      
4. Java                                                            
5. Selenium Webdriver                                              
6. TestNG                                                          
7. Cucumber

## GUI Tests:
## Tested below scenarios in the application (Frontend)
1. Validate the working of Register Account functionality
2. Validate the working of Login functionality
3. Validate the working of Logout functionality
4. Validate the working of Forgot Password functionality
5. Validate the working of Search functionality
6. Validate the working of Product Compare functionality
7. Validate the Product Display Page functionality for the different types of Products
8. Validate the working of 'Add to Cart' functionality
9. Validate the working of 'Wish List' functionality
10. Validate the working of 'Shopping Cart' functionality
11. Validate the working of Home Page functionality
12. Validate the working of Checkout functionality
13. Validate the My Account functionality
14. Validate the working of My Account > Account Information functionality
15. Validate the working of My Account > 'Change Password' functionality
16. Validate the working of My Account > 'Address Book' functionality
17. Validate the working of My Orders > 'Order History' functionality
18. Validate the working of My Orders > 'Order Information' functionality
19. Validate the working of My Orders > 'Product Returns' functionality
20. Validate the working of My Orders > 'Downloads' functionality
21. Validate the working of My Orders > 'Reward Points' functionality
22. Validate the working of My Orders > 'Returned Requests' functionality
23. Validate the working of My Orders > 'Your Transactions' functionality
24. Validate the working of My Orders > 'Recurring Payments' functionality
25. Validate the working of 'Affiliate' functionality
26. Validate the working of 'Newsletter' functionality
27. Validate the working of 'Contact Us' page functionality
28. Validate the working of 'Gift Certificate' page functionality
29. Validate the working of 'Special Offers' page functionality
30. Validate the working of 'Header' options, 'Menu' options and 'Footer' options
31. Validate the complete Application functionality for different currencies

 ## Requried Installations
1) Flow these Link to Download JDK : https://drive.google.com/file/d/1OaxJvruKHIlp5gmt7w6iA69tAfGrOIOa/view?usp=sharing
2) Eclipse Version: 2020-12 (4.18) & lower versions supporting TestNG
3) TestNG Version: 7.2.0 latest (or lower versions)
    Step1) Download Java8 and install it (If not done so far)
    Step2) Download Eclipse and install on Windows. 
           You can see Eclipse Downloads (Zip File) in below link.
           https://www.eclipse.org/downloads/packages/
    Step3) Once you Download Zip File, Extract Zip File and you can see
    Step4) Launch Eclipse by clicking on eclipse.exe
    Step5) Once Eclipse is Launched, Go to Help→ Install New Software
           Eclipse files as below.
    Step6) Click on Add button and provide Name & Location details.
           Link: https://testng.org/testng-eclipse-update-site/7.2.0
    Step7) Select TestNG checkbox then follow the below screens.
    Step8) Eclipse will be restarted. After that go to Window Menu→
           Preferences
           You can see TestNG option in the list. (Means Installation successful).

3) XAMPP follow these steps : https://drive.google.com/file/d/1o9YYr5hZmhIlAxpOvgew4XzgriYIBIKo/view?usp=sharing
4) Use these test cases: https://docs.google.com/spreadsheets/d/1ikSwGBDhO4aiJZw26A6x1dJuHtlAuSTW/edit?usp=sharing&ouid=103801190138918883992&rtpof=true&sd=true

## Development of Hybrid Driven Framework

1) Test case: Account Registration
1.1: Create BasePage under "pageObjects" which includes only constructor. This will be invoked by
every Page Object Class constructor (Re-usability).
1.2: Create Page Object Classes for HomePage & RegistrationPage under pageObjects package.
(These classes extends from BasePage).
1.3: Create AccountRegistrationTest under "testCases"
1.4: Create BaseClass under testBase package and copy re-usable methods.
1.5: Create re-usable methods to generate random numbers and strings in BaseClass.

2) Adding logs to test case (log4j2)
2.1: Add log4j2.xml file under src/test/resoures.
2.2: Update BaseClass.
2.3: Add log statements to AccountRegistrationTest.

3) Run Tests on Desired Browser/Cross Browser/Parallel
3.1: Create testng.xml file to Run Test Cases and parameterize browser name to BaseClass
→setup() method.
3.2: Update BaseClass →setup() method, launch browser based on condition.
3.3: Maintain separate xml to run tests multiple browsers parallelly.

4) Read Common values from config.properties file.
4.1: Add config.properties file under src/test/resoures.
4.2: Update BaseClass →setup() method, add script to load config.properties file
4.3: Replace hard coded values in Test Cases like url, username, password etc...

5) Add Extent Reports to Project
5.1: Create ExtentReportUtility utility class under utilities package.
5.2: Add captureScreen() method in BaseClass
5.3: Add ExtentReportUtility (Listener class) entry in testng.xml file.
5.4: Make sure WebDriver is static in BaseClass, we refer same driver instance in ExtentReportUtility.

6) Login Test Case
6.1: Create and update page object classes.
LoginPage, MyAccountPage – new classes
HomePage – update by adding login link element
6.2: Create LoginTest
6.3: Add entry testng.xml


7) Data Driven Login Test
7.1: Prepare test data in Excel, place the excel file inside the testData folder.
7.2: Create ExcelUtility class under utilities package.
7.3: Update Page Object class MyAccountPage , add logout link element)
7.4 : Create DataProviders class in utilities package to maintain data providers for data driven tests.
7.5: Create LoginDataDrivenTest under testCases package.
7.5: Add an Entry in testng.xml file


8) Grouping Tests.
8.1: Add all test cases into specific group.
Sanity
   TC_002_Login
Regression
    TC_001_AccountRegistration
Master
   TC_002_Login
   TC_001_AccountRegistration
8.2: Also add BaseClass methods setup() & teardown() to all groups.
8.3: Create separate TestNG xml file(grouping.xml) to run groups and include groups which we want to execute.

9) Run Failed Tests.
test-output→testng-failed.xml
10) Run Tests using Maven pom.xml, Command Prompt & run.bat file.
11) Push the Code to Git & GitHub Repository
12) Run Tests using Jenkins.

## Folder structure
https://drive.google.com/file/d/1_nIkYR8MK0oPAoNNwaCqzsarAKsctIgg/view?usp=sharing























