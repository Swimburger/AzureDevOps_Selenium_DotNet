Build: [![Build Status](https://dev.azure.com/swimburger/AzureDevOps%20Selenium%20DotNet/_apis/build/status/Swimburger.AzureDevOps_Selenium_DotNet?branchName=master)](https://dev.azure.com/swimburger/AzureDevOps%20Selenium%20DotNet/_build/latest?definitionId=12&branchName=master)

QA Deploy (fake):
[![QA Deploy (Fake)](https://vsrm.dev.azure.com/swimburger/_apis/public/Release/badge/4a5cc01b-14d7-4a4f-bfac-819595a092f7/1/1)](https://dev.azure.com/swimburger/AzureDevOps%20Selenium%20DotNet/_release?view=mine&definitionId=1)   
Verify QA Ubuntu:
[![Verify QA Ubuntu](https://vsrm.dev.azure.com/swimburger/_apis/public/Release/badge/4a5cc01b-14d7-4a4f-bfac-819595a092f7/1/2)](https://dev.azure.com/swimburger/AzureDevOps%20Selenium%20DotNet/_release?view=mine&definitionId=1)   
Verify QA Windows:
[![Verify QA Windows](https://vsrm.dev.azure.com/swimburger/_apis/public/Release/badge/4a5cc01b-14d7-4a4f-bfac-819595a092f7/1/3)](https://dev.azure.com/swimburger/AzureDevOps%20Selenium%20DotNet/_release?view=mine&definitionId=1)

# AzureDevOps Selenium DotNet
This is the reference repository for the following blog posts on [swimburger.net](https://www.swimburger.net):
* [How to UI test using Selenium and .NET Core on Windows, Ubuntu, and maybe MacOS? 🤷‍♀️🤷‍♂️](https://www.swimburger.net/blog/dotnet/how-to-ui-test-using-selenium-and-net-core-on-windows-ubuntu-and-maybe-macos)
* [How to run .NET Core Selenium UI tests on Azure DevOps Pipelines Windows/Ubuntu agents? 🚀](https://www.swimburger.net/blog/dotnet/how-to-run-net-core-selenium-ui-tests-on-azure-devops-pipelines)

## Prerequisites
* [.NET Core SDK](https://dotnet.microsoft.com/download/dotnet-core) (2.2)
* Windows, Linux, or MacOS dev machine
* Chrome/Chromium web browser
* [Chrome WebDriver](https://chromedriver.chromium.org/downloads) (make sure the driver version matches the browser version)

## How to run
To run the tests, use dotnet cli with the settings parameter pointing to .runsettings.
```
cd Demo.SeleniumTests
dotnet test -s .runsettings
```

The .runsettings allows you to specify test parameters, in this case `webAppUrl` and `headless`.
On a shell only OS (no gui), you'll need to use headless.
