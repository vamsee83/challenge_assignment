-Installation and running instructions
 1. Install Maven 3.3+ and java sdk 1.8+
 2. Set the enviornment variable "JAVA_HOME" to <Java installation>(ex:C:\Program Files\Java\jdk1.8.0_25) directory
 3. Update the system path with Maven path <Maven Installation>\bin directory
 4. check from command prompt if maven is working with "mvn -version" it should print the maven version
 5. Download project from https://github.com/vamsee83/challenge_assignment.git
 5. Copy the settings.xml from the project directory to <user home>\.m2 (ex: C:\Users\vuppuv\.m2)
 6. Finally, run the project with command "mvn -U clean install". It will build the poroject(download selenium, chromedriver etc) and run tests.
 
 Once test's complete you will see the below output in command prompt
 **********Dealer Contact************
contact name:Chris Hales
contact address: 1230 Santa Monica Blvd
contact address: Santa Monica, CA 90404
email address: chrish@smford.com
phonenumber: (310) 451-1588
**********************
Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 38.779 sec - in TestSuite
Results :
Tests run: 2, Failures: 0, Errors: 0, Skipped: 0

The html report is available at ./target/surefire-reports/emailable-report.html
TestNG testcases file: src/test/resources/AutoBlog_testNG.xml

-brief explanation of your approach

1. Build tool: Maven
2. Framework: TestNG
3. Programming language: Java
4. Tools: Selenium webdriver
The tests are automated using Java programming language and selenium webdriver API's. The framework is TestNG. I used PageObject pattern, which provides more flexibility for future changes
and keep things organized. 
Maven build tool will take care of downloading all dependencies.

-future enhancements
 1. I was planning to use spring framework which will take care of dependency injection of pageObjects into tests. As i could not get it working in this short time frame i removed it. Adding Spring framework will be future enhancement. 
 2. Cross browser support, right now the tests are running in chrome browser. We need run them in IE,firefox etc and make sure thier is no issues.
 
-compromises made
 1. I added basic checks in each page, if i had more time i would like to add more checks to verify the data in each page.
