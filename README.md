# POM
Using Selenium WebDriver and TestNG framework and Maven dependency

Page Object Model (Page Chaining Model)
- Design pattern approach
- Data Driven Framework
- TestNG

pages
1. Page Layer (Page Lib)

LoginPage -- WebObjects/WebElements -- Actions/Methods(features) 

HomePage
RegistrationPage -- clickOnSignInLink(); fillReqForm(); checkLogo(); footerLink()
SearchPage
AddToCartPage
PaymentPage

test
2. Test Layer - TestNG -- annotations
LogInPageTest.java
HomePageTeat.java
RegPageTest.java

base
3. There is a java parent class TestBase.java (WebDriver dr = new ChromeDriver()) connecting 1 and 2.
	maximizeWindow() - pageloadTimePut() - impiciWait() - deleteAllCookies() - get(url)

config
4. Envornment Vars
	Config.properties - URL - UserName - Password - Browser
	
testdata
5. TestData.xlsx

util
6. TestUtil.java
	Screenshot - sendMail() - commonUtil() - Generic Functions

test-output/reports

7. Test Reports: Pass/Fail
	HTML - TestNG - XML reports - Extent reports
	
Java
Selenium WenDriver
TestNG
Maven
Apache POI API
Extent Report/TestNG report
Log4j API
Jenkins - CI
GIT - Repo
GRID - Parallel Testing
Browsers - FF/Chrome/IE
Mac/Windows/Linux
VMs/SourceLabs/BrowseStack/Local
