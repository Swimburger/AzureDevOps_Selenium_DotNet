# AzureDevOps Selenium DotNet
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
