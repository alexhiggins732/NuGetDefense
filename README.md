# [NuGetDefense](https://digitalcoyote.github.io/NuGetDefense/)

[![Join the chat at https://gitter.im/NuGetDefense/community](https://badges.gitter.im/NuGetDefense/community.svg)](https://gitter.im/NuGetDefense/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)  [![NuGet version](https://badge.fury.io/nu/NugetDefense.svg)](https://badge.fury.io/nu/NugetDefense)

An MSBuildTask that checks for known vulnerabilities. Inspired by [OWASP SafeNuGet](https://github.com/OWASP/SafeNuGet).
  
## Docs
View the full documentation for NuGetDefense [here](https://digitalcoyote.github.io/NuGetDefense/)
  
## Features  
* Uses Multiple Sources to check for known vulnerabilities in third-party libraries (NuGet packages)
  * [OSS Index](https://ossindex.sonatype.org/)
  * [National Vulnerability Database](https://nvd.nist.gov/) (Optionally Self-Updating)
* Simple installation/configuration: the [NuGet Package](https://www.nuget.org/packages/NuGetDefense/) is all you need.
* Allow breaking the build based on severity of vulnerability.
* Ignore specific vulnerabilities/packages.
* Blacklisting NuGet Packages
* Whitelisting NuGet Packages
* MIT Licensed

## Planned Features
* Checking Dependencies based on the versions that were installed when the project was built.

## Requirements
  Currently NuGetDefense is built only in .Net Core 3.1 so you will need the runtime/SDK installed.

## How does it work?
  NuGetDefense is a bundled dotnet tool that runs using an [MSBuild ExecTask](https://docs.microsoft.com/en-us/visualstudio/msbuild/exec-task?view=vs-2019) after your project finishes building.

    
## Love it? Support it!
You can sponsor this project on [Github](https://github.com/sponsors/digitalcoyote) and [Patreon](https://www.patreon.com/codingcoyote). The funds will be used to pay for software licenses and cloud/hardware costs that keep my projects running.
