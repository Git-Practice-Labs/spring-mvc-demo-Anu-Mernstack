Step-by-Step: Spring Boot MVC using Eclipse + Maven
________________________________________
 
 STEP 1: Create a Maven Project
1.	Go to File
2.	Click New
3.	Click Project…
 A dialog opens
________________________________________
In the Wizard:
4.	Select Maven
5.	Select Maven Project
6.	Click Next
________________________________________
Maven Project Settings:
7.	 Check Create a simple project (skip archetype selection)
8.	Click Next
________________________________________
STEP 2: Enter Maven Project Details
Fill the fields exactly like this (you may change names later):
Field		Value
Group Id	com.example
Artifact Id	spring-mvc-demo
Version	0.0.1-SNAPSHOT
Packaging	jar
Name		spring-mvc-demo
9.	Click Finish
Maven project is created
________________________________________
 STEP 3: Convert to Spring Boot (pom.xml)
Open pom.xml
1.	Expand project → open pom.xml
2.	Replace its content with this MINIMAL Spring Boot pom.xml
3.	Save the file
4.	Right-click project → Maven → Update Project
5.	Click OK
 Maven downloads dependencies
________________________________________
 STEP 4: Create Main Spring Boot Class
Create Package
1.	Right-click src/main/java
2.	Click New → Package
3.	Name it:
com.example.demo
________________________________________
Create Main Class
4.	Right-click the package
5.	Click New → Class
6.	Class name:
SpringMvcDemoApplication
7.	Click Finish
________________________________________
Paste Code: SpringMvcDemoApplication

 STEP 5: Create Controller
1.	Right-click com.example.demo
2.	New → Package
3.	Name:
controller
________________________________________
4.	Right-click controller
5.	New → Class
6.	Name:
HelloController
Paste Code for HelloController

________________________________________
 STEP 6: Create View (HTML)
1.	Right-click src/main/resources
2.	New → Folder
3.	Name:
templates
_______________________________________
4.	Right-click templates
5.	New → File
6.	Name:
hello.html
Paste HTML code given:
________________________________________
STEP 7: Run the Application
Method 1 
Right-click SpringMvcDemoApplication.java
1.	Click Run As
2.	Click Java Application
________________________________________
Method 2 (Maven)
1.	Right-click project
2.	Run As → Maven build
3.	Goal:
spring-boot:run
4.	Click Run
________________________________________
 STEP 8: Test in Browser
Open browser and go to:
http://localhost:8080/hello
You should see:
Hello from Spring Boot MVC!

