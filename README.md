# Restful-booker (API test using Postman and newman reports generated)
# Reports Preview
## htmlextra report
![alt text](https://github.com/ntdsrd/restful-booker-postman/blob/master/preview/htmlextra.png)
## allure report
![alt text](https://github.com/ntdsrd/restful-booker-postman/blob/master/preview/allure.png)
# How to open reports
- Clone project
  ```
  git clone https://github.com/ntdsrd/restful-booker-postman.git
  ```
## htmlextra report
- Open htmlextra/report.html on your browser
## allure report
> Dependencies: npm, allure-commandline
- Install npm (depend on your os, check npm if exists: npm -v)
- Install allure-commandline
  ```
  npm install -g --save-dev allure-commandline
  ```
- Open allure report
  ```
  allure open allure/allure-report
  ```
  or
  ```
  allure serve allure/allure-results
  ```
  > If your browser is not opened. Click to link as `Server started at <http://192.168.1.112:38877/>. Press <Ctrl+C> to exit`
