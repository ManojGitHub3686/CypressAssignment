Read Me!!!!

Cypress assignment to verify https://www.ltimindtree.com/ web pages

About Project:
Testing a web page i.e., https://www.ltimindtree.com/ using Cypress tool and JavaScript as a language on Chrome browser

How to install the project locally:
Information: "node-module" folder is not included because the folder can be very heavy (several hundreds of Mb), and it would cause your pushes to be very long, and not up-to-date with your semver.
To install "node_modules" folder, you have to run below commands after you selected yourr folder in IDE i.e., Visual Studio Code. 
Open VSC terminal and run
"npm install cypress --save-dev" 
It will reinstall cypress and create "node_modules" folder.


1. Download project from GitHub (.zip format).  
2. Extract the folder on local machine . 
3. Open Visual Studio Code IDE -> Select Open folder -> Select the extracted folder 
4. Verify 'Package.json' -> Scripts section have below line is added. It will help you to run your test from terminal.
"cy-test": "npx cypress run -s .\cypress\e2e\stepdef.feature -b chrome --env allure=true"

Note: Test would run on chrome browser in headless mode.

How to run tests:
1. Open Visual Studio Code terminal and type in below commands.

a. npm run cy-test -> It will run the tests in command prompt and shows the result 
b. npm run allure:report (Pre-requisite: Java 8+ needs to be install on local machine) 
c. npx allure open -> Check the report on browser

2. If you have "Cypress" tool install then instead of step 1, run below command in terminal 
a. npx cypress open -> It will open Cypress tool 
b. Select desired browser 
c. Select 'stepdef.feature' spec file -> It will run the test on selected browser
