# API Performance Testing Framework using JMeter

## Project Overview

This project demonstrates API Performance Testing using Apache JMeter.

The framework is designed to simulate virtual users and measure:
- response time
- throughput
- error percentage
- scalability

The project includes:
- API load testing
- assertions
- parameterization
- HTML reporting
- reusable test plans

## Tools & Technologies

- Apache JMeter
- Java
- HTTP/HTTPS APIs
- GitHub
- HTML Dashboard Reports

## Project Structure
```
performance-testing-framework/
│
├── test-plans/
├── test-data/
├── reports/
├── screenshots/
├── README.md
```

## Test Scenario

API Tested:
GET https://reqres.in/api/users?page=2

Load Profile:
- Virtual Users: 50
- Ramp-Up Time: 10 seconds
- Loop Count: 5

Assertions:
- Status Code = 200

## Report Generation - we can get both .csv and beautiful html  reports 

.\jmeter.bat -n -t PerformaceTestProjectSample.jmx -l results.csv

.\jmeter.bat -g results.csv -o html-report

# How to Execute

## Prerequisites
- Java Installed
- Apache JMeter Installed
- Set JAVA_HOME
- Add JMeter bin folder to PATH

## Clone Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
```

## Navigate to Project Folder

```bash
cd your-repo-name
```

## Run JMeter Test

```bash
jmeter -n -t TestPlan.jmx -l result.jtl
```

## Generate HTML Report

```bash
jmeter -g result.jtl -o HTMLReport
```

## Open Report

Open `index.html` inside the `HTMLReport` folder.
