# Windows Security Baseline

Windows Baseline is a collection of security improvements compiled by microsoft that apply recommended base level of security beyond what it configured OOB (Out of the Box).

Requirements: Windows 10/11 Pro

Typically this would be deployed via Group Policy or MDM such as Intune, however Microsoft also provides premade local installation scripts for installing Microsoft Baseline on your local device. 

Read more about Windows Security Baseline Here: https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-security-configuration-framework/windows-security-baselines

This guide is intended to walk you through how to install this locally on your device.

1. Download the Toolkit here and just select the OS version you require: https://www.microsoft.com/en-us/download/details.aspx?id=55319
2. Extract the files to a folder
3. Open Powershell as an Admin
4. Use 'CD' and navigate to the downloaded folder > scripts
5. Run the local install file with the following arguments

.\Baseline-LocalInstall.ps1 -win10nondomainjoined

6. Once complete, restart your computer.
