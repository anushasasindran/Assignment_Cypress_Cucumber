# **CypressBDDCucumber**
This repository features a comprehensive Cypress framework integrated with BDD using Cucumber, designed for end-to-end testing of a sample project. 
# **Description**
This automates this web page - https://practice.expandtesting.com/notes/app  
The scenarios covered are Registrartion, Login and Add notes
**Cucumber BDD** : Using cucumber feature files and step definitions files.  
**Data-driven testing**: is achieved using cucumber feature files and JSON files for managing input and output data.  
**Advanced Reporting**: Integration with Mochaawesome for detailed and informative test reports.  
**Efficient Test Organization**: Using the Page Object Model for maintaining and managing UI tests.  

# **Pre-requistes**  
**Operating System**: Cypress is a desktop application that is installed on your computer. It supports macOS, Linux, and Windows.  
**Node.js**: Cypress is a Node.js application. Ensure you have Node.js (and npm) installed. A version of 10 or above is recommended.  
**Supported Browsers**: While Cypress can run tests in any browser installed on your machine, it's good to have Chrome, Firefox, Edge installed and updated to latest versions.  
**Development Environment**: Code editor(preferably Visual studio code).  
# **Installation**  
**Create a folder**: Create a folder in your system. Open the folder in VS or any command line tool.  
**Commands**  
npm init – After this command is ran it created package.json file in folder   
npm install cypress --save-dev : This installs the latest cypress version  
npm install cypress@12.16.0 : If you want any specific cypress version to download  
	Node modules folder is created once the cypress is installed  
Install Cucumber with Cypress using npm install --save-dev cypress-cucumber-preprocessor.
npx cypress open : This open the cypress test runner and to configure framework   
**Feature Files**  
Write Gherkin syntax in .feature files located in the cypress/e2e/project/features.  
**Step Definitions**  
Implement step definitions in JavaScript files within the cypress/e2e/project/stepDefinitions folder.  
**Configuration**  
Update cypress.json and package.json to include cucumber preprocessor settings.  

# **How to run cypress tests**  
**Using cypress test runner** : npx cypress open command to open test runner. Click on each spec files and run it.   
**Using command line headless mode**: npx cypress runs all the features under the e2e folder one by one based on the order in that folder.   
**Using command line headless mode to run a single file**: npx cypress run --spec “feature file path” runs a single file from the file path mentioned.    
**Using command line headed mode to run in specific browsers** : "npx cypress run --headed --browser <broswername> --spec ‘feature files folder’”  
# *Reporting**  
Mochawesome reports are used.  
Install by using the below commands:  
npm install mochawesome --save-dev  
npm install mochawesome-merge --save-dev  
npm install mochawesome-report-generator --save-dev  
# **Scripts**  
The scripts to run are given under Scripts on Package.json file(to run in test runner and Commandline in headed and non-headed).  
npm run clean-up(to clean the previous results)
npm run UICLtest(to run the UI tests in CL)  
npm run mochawesome-merge(to generate the reports)





