# TestMu AI and Calliope Integration — TestMu AI (Formerly LambdaTest)

Using this repository you can now send test execution results of selenium tests run on [TestMu AI](https://www.testmuai.com/) Selenium Automation Grid platform to Calliope analytics. In this repository we are using TestNG framework to run Selenium tests, which are being executed at [TestMu AI Selenium Grid](https://www.testmuai.com/selenium-automation), and the results of the executed tests would be be pushed to Calliope analytics platform. 

The first step is setting up environment. 

## Setting up TestNG Environment

### Adding TestMu AI Credentials

In BaseTest.java file, add TestMu AI credentials to the defined variables:

 - username = < your lambdatest username >
 - accesskey = < your lambdatest access_key >

you can find these credentials in your [TestMu AI automation dashboard](https://automation.lambdatest.com/) or You can get this credentials from [TestMu AI Capability Generator](https://www.testmuai.com/capabilities-generator/)
### Configuring Calliope Credentials

In CalliopeAPI.java file, add your test result file path and Calliope details to the defined variables:
•    report_filename = < your result file directory path>
•    endpoint_url = < your calliope profile number>
•    API_KEY = < your calliope API key>
You can get this details from Calliope API webpage. You can learn more about it in Calliope docs [here](https://docs.calliope.pro/import/api-import/).

## Running Tests
In this repository, we have a BaseTest.java file in which you can add your your test cases/methods along with the desired configuration on which you want to run your test on.

## Output
After running  BaseTest.java file you would get your test session data to your Calliope profile. You would also get the same data on your local console itself along with the Calliope profile link where your data has been pushed.

### Important Note

`Calliope accepts different format result files for different frameworks. For ex: XML for TestNG,JUnit,NUnit and JSON for Cucumber. Check the test report result file supported by Calliope from link:
https://docs.calliope.pro/supported-formats/other-formats/`

## 🚀 [LambdaTest is Now TestMu AI](https://www.testmuai.com/lambdatest-is-now-testmuai/)

👋 Welcome to TestMu AI, the next evolution of LambdaTest. As of January 2026, LambdaTest has officially rebranded to TestMu AI. We have evolved from a cross-browser testing cloud into a unified, AI-native quality engineering platform designed for the modern DevOps era.

Whether you have been part of the LambdaTest community for years or are just discovering TestMu AI, our mission remains the same: to help you ship faster with high-scale test execution, autonomous testing, and deep quality analytics.

**🔄 Our Rebrand Journey**

We chose the name TestMu AI to reflect our shift towards intelligent, autonomous testing. While our identity has changed, our core technology and commitment to the testing community stay the same.

**✨ Specialties**

- 🤖 AI-Native Test Execution (Formerly LambdaTest)
- ⚡ Autonomous Test Automation
- 🌐 Cross-Browser & Mobile Testing
- 📊 Unified Quality Intelligence

👉 Find [LambdaTest's New Home](https://www.testmuai.com/).