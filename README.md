# SecureBank Manual Testing Project

## Project Overview
SecureBank is a secure online banking platform developed to provide safe and efficient digital banking services. This project used manual testing to check if the platform works correctly, is secure, and performs well.



## Testing Scope
The manual testing process covered various aspects of the SecureBank platform, focusing on:
- **Functionality Testing:** Verification of core banking features and user interface components.
- **Security Testing:** Identifying potential vulnerabilities.
- **Usability Testing:** Ensuring an intuitive and user-friendly experience.
- **Cross-Browser Testing:** Validating compatibility across multiple browsers.

## Testing Activities Performed

### Test Plan Creation

Google Drive Link: https://drive.google.com/drive/u/5/folders/12RPU15GDlBRR66RHudkBW9HG8IoW-CNt

- Developed a structured **test plan** outlining:
  - Testing objectives
  - Scope
  - Test items
  - Features to be tested
  - Features not to be tested
  - Test Environment
  - Schedule

### Mindmap
- Designed a **mind map** to visualize:
  - Testing strategy
  - Feature coverage
![SecureBank Test Image](https://drive.google.com/drive/u/5/folders/19SW5oC-cZrxinvUlOzjH3srV_ffOe1BO)
<img src="https://drive.google.com/drive/u/5/folders/19SW5oC-cZrxinvUlOzjH3srV_ffOe1BO" alt="SecureBank Test Image_Graph" width="500"/>

  ### Test Scenarios
- Defined multiple **test scenarios** to validate:
  - Critical functionalities
  - Edge cases
  - Boundary Value testing
  - Negative testing
  
### Test Case Writing
- Created detailed test cases covering various modules of the **SecureBank** application.

### Test Metrics
- Collected and analyzed **test metrics** to assess:
  - Test coverage
  - Test execution progress

<img src="https://drive.google.com/uc?id=1Vk7w84RBuLYz6KOwFqZaW0XP8rtsJXyG" alt="SecureBank Test Image_Graph" width="500"/>  

### Bug Reports
- Documented identified **defects** with:
  - Severity
  - Priority
  - Steps to reproduce
  - For efficient tracking and resolution
<img src="https://drive.google.com/uc?id=1Vk7w84RBuLYz6KOwFqZaW0XP8rtsJXyG" alt="SecureBank Test Image_Graph" width="500"/>

### Tools Used
- Test Management Tool: Excel Sheets / Google Sheets
- Mind Mapping Tool: XMind 


### Key Outcomes
- Identified and reported critical bugs affecting functionality and security.
- Achieved comprehensive test coverage through detailed test cases and scenarios.
- Ensured the platform's compatibility across various browsers and devices.


## Conclusion
This manual testing project for SecureBank has successfully validated the platform's core functionalities and security measures. The documentation, including test cases, scenarios, mind map, test summary report, test metrics, and bug reports, has been prepared to assist in continuous quality improvement.

## Test Report Summary

![SecureBank Test Image](https://drive.google.com/uc?id=1jmW2DDJ7o5DdMslVYbFrv0yHG21jrjIm)

<img src="https://drive.google.com/uc?id=1Vk7w84RBuLYz6KOwFqZaW0XP8rtsJXyG" alt="SecureBank Test Image_Graph" width="500"/>

readme file added
# SecureBank
[![Docker Automated](https://img.shields.io/docker/cloud/automated/ssrd/securebank.svg)](https://hub.docker.com/r/ssrd/securebank)
[![Docker Build status](https://img.shields.io/docker/cloud/build/ssrd/securebank.svg)](https://hub.docker.com/r/ssrd/securebank/builds)
[![License](https://img.shields.io/github/license/ssrdio/SecureBank)](https://github.com/ssrdio/SecureBank/blob/master/LICENSE)

[![](https://sonarcloud.io/api/project_badges/measure?project=ssrdio_SecureBank&branch=master&metric=vulnerabilities)](https://sonarcloud.io/dashboard/?id=ssrdio_SecureBank&branch=master) 
[![](https://sonarcloud.io/api/project_badges/measure?project=ssrdio_SecureBank&branch=master&metric=bugs)](https://sonarcloud.io/dashboard/?id=ssrdio_SecureBank&branch=master) 
[![](https://sonarcloud.io/api/project_badges/measure?project=ssrdio_SecureBank&branch=master&metric=code_smells)](https://sonarcloud.io/dashboard/?id=ssrdio_SecureBank&branch=master) 

SecureBank is a FinTech application which contains all OWASP TOP 10 security vulnerabilities along with some other security flaws found in real-world applications.

You can read more about SecureBank and OWASP top 10 vulnerabilities [here](https://ssrd.gitbook.io/securebank/).
![alt text](https://raw.githubusercontent.com/ssrdio/SecureBank/master/preview.gif "SecureBankPreview")

# Setup
> You can setup SecureBank application from source code, or simply pull it from [Docker Hub](https://hub.docker.com/r/ssrd/securebank).

# Infrastructure
On the image below you can review how the application is built from the infrastructure point of view.
![alt text](https://raw.githubusercontent.com/ssrdio/SecureBank/master/infra.png "Docker infrastructure")

## From source
> Make sure that you have Microsoft SQL Server DB available. You can install or run it inside docker.

1. Install [.NET 5.0 SDK](https://dotnet.microsoft.com/download/dotnet/5.0)
2. Install [Visual Studio 2019](https://visualstudio.microsoft.com/downloads/) or just run with  [Visual Studio Code](https://code.visualstudio.com/download)
3. Clone from GitHub
4. Navigate to directory SecureBank -> src
5. `dotnet run` or open solution in IDE and run there 


## From Docker
1. Install [Docker](https://docs.docker.com/get-docker/)
2. Execute `docker run -d -p 80:80 -p 5000:5000 -p 1080:1080 -e 'SeedingSettings:Admin=admin@ssrd.io' -e 'SeedingSettings:AdminPassword=admin' ssrd/securebank`
3. Open [http://localhost:80](http://localhost:80)
