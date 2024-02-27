# Restful-booker (API test using Postman and newman reports generated)

## Reports Preview

### htmlextra report

![htmlextra](https://github.com/ntdsrd/restful-booker-postman/blob/master/preview/htmlextra.png)

### allure report

![allure](https://github.com/ntdsrd/restful-booker-postman/blob/master/preview/allure.png)

## Open project with Postman

Open collection `restful-booker.postman_collection.json` and environment `prod.postman_environment.json` by Postman to run the test

Click on each request and go to Tests to see test scripts

## Open reports

Clone project

```
git clone https://github.com/ntdsrd/restful-booker-postman.git
```

### htmlextra report

Open htmlextra/report.html on your browser

### allure report

> Dependencies: npm, allure-commandline

Install npm (depending on your OS, check npm if it exists: npm -v)

Install allure-commandline

```
npm install -g --save-dev allure-commandline
```

Open allure report

```
allure open allure/allure-report
```

or

```
allure serve allure/allure-results
```

> If your browser is not opened, click on the link as `Server started at <http://192.168.1.../>. Press <Ctrl+C> to exit`

## Generate reports

> Dependencies: npm, newman, newman-reporter-htmlextra, newman-reporter-allure

Install npm (depending on your OS, check npm if it exists: npm -v)

Install newman

```
npm install -g newman
```

### htmlextra report

Install newman-reporter-htmlextra

```
npm install -g newman-reporter-htmlextra
```

Generate htmlextra report

```
newman run <collection> -e <environment> -r htmlextra --reporter-htmlextra-export <path>
```

> Path: filename -> htmlextra/report.html

### allure report

Install newman-reporter-allure

```
npm install -g newman-reporter-allure
```

Generate allure results

```
newman run <collection> -e <environment> -r allure --reporter-allure-export <path>
```

> Path: folder contains allure results -> allure/allure-results

Install allure-commandline

```
npm install -g --save-dev allure-commandline
```

Generate allure report

```
cd <path-of-allure-results>
```

```
allure generate <path>
```

> Path: folder contains allure report -> allure-report
