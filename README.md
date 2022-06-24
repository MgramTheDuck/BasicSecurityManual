# Mgram's Recommendations for Basic Home Security

These are a handfull of simple and easy recommendations that I have pulled together over the years to improve your home security on a windows PC and help you feel confident and safe online.

> Background: I have been working in the IT Industry for a little over 6 years, covering roles from Helpdesk support, Network Engineering and more recently Cloud Security and consulting. As such I have worked on a wide variety of platforms, applications and tools. This guide is a collection of some of the basic recommendations which I would make to anyone who wants to have a bit more control over their own personal security and their online footprint.

NOTE: This is a work-in-progress and I will be adding more content to this over time. If you see any errors or mistakes, please feel free to create a PR or contact me directly. My details are in my Bio.

## 1 Account Management

### 1.1 Use a Password Manager (Paid/Free)

Re-using passwords is a very quick way to have all your accounts hacked, If so much as one service is breached you might find yourself in a lot of trouble very quickly. I strongly recommend using a password manager, to store passwords and ensure you create unique passwords for every service.

- [Bitwarden](https://bitwarden.com/) (Cloud Service, Paid, Open Source)
- [Dashlane](https://www.dashlane.com/) (Cloud Service, Paid)
- [KeePass](https://keepass.info) (Stored on your PC, Free)

DO NOT keep passwords in a text file/word document/etc on your PC, this is the first thing potential hackers will look for.

### 1.2 Use Good Passwords

Good passwords are suprisingly hard to come by, but they don't need to be difficult. Here is a very simple formula for creating complex and memorable passwords.

- Two words
- One symbol between the words
- One words in all CAPS
- 2 numbers at the end

Examples:

- summer-CAKES88
- GREEN@clouds44
- bright!GLASS23

These passwords will meet 99% of requirements and are easy to remember.

DO NOT:
- Use sequential passwords (password1, password2)
- Use dates or birthdays
- Use names of people you know personally

### 1.3 Use Multi-factor authentication

If it is available, you should ALWAYS use Multi-factor authentication (AKA: 2-Factor Authentication). This should be either an SMS, code or notification on your phone. 

Passwords will inevitably get breached, but MFA is the No.1 method to prevent account breaches and has saved me more than once.

### 1.4 Clean up old accounts

Its very easy to lose track of how many websites and services you have signed up for in the past, any one of these could prove a possible vulnerability and opportunity for someone to get hold of your data or initiate identity theft. 

When you ar no longer using a website or service, you should delete your account, this is the best way to ensure it cannot be used against you.

A good tool to find websites you are previously signed into is [WhatsMyName.app](https://whatsmyname.app) which will take your username and locate any website or service where that username was previously used to create an account.

## 2 Windows Security

These improvements are for your home computer and include recommendations for security settings and antivirus features.

Many of these will not affect your day-to-day use but will greatly improve secuirty and reduce your chances of being affected by malware or ransomware.

### 2.1 Use Cloud Storage (Free/Paid+)

Every disaster recovery solution begins with backups, and keeping your important data backed up in a cloud-based storage platform is the best place to start. Many services are free for the first 5-10GB of storage, this should be more than enough for any of your important personal document.

As a bare minimum, you should have at least one cloud storage location for your most important files, this platform should also have:
- A Secure Password
- Multi-factor authentication

**A general rule of thumb: If you cannot re-download it, it should be stored in the cloud**

This should be for storing anything of critical importance:
- Medical Documents
- ID Documents
- Legal Documents
- Contracts/Certifications
- Family Documents/Photos/etc

Having a system like this is the best way to ensure that no matter what happens, you will always have your most important files.

Some good options are:
- OneDrive (5GB Free)
- Google Drive (15GB Free, 100GB @ $2.99AUD/month)
- Dropbox (2GB Free)

### 2.2 Use BitLocker (Windows 10/11 Pro)

Bitlocker is a built-in feature for windows that allows you to encrypt your drives, this is important for laptops and portable devices. Unencrypted drives can be connected to a different computer and the files copied directly off them without any extra effort. Using bitlocker will ensure that your files are safe, even if your drive falls into someone elses hands.

To enable bitlocker:
1. Open start menu
2. Type `Bitlocker`
3. Take the first option `Manage Bitlocker`
4. For each drive, select `Turn on bitlocker`
5. Follow the steps to enable bitlocker, make sure you make a copy of the recovery key.

![image](https://user-images.githubusercontent.com/85346345/175436088-64ec346d-e107-42eb-9a32-26df9a1255c1.png)

You will be provided an opportunity to backup the "recovery key", this is important if you decide to move the drive to another computer, you will be prompted to enter the "recovery key" to get access to the drive again.

I suggest you make a copy of this and store it securely in a cloud-based file storage (OneDrive, Google Drive) as mentioned in 2.1

### 2.3 Setup Windows Defender Correctly (Windows Security App)

Since Windows 10, Microsoft has developed a very strong and advance Antivirus/Antimalware platform built directly into windows, this is now one of the leading software options for AV solutions. Many large enterprises now use Windows Security as their primary AV solution.

To get the most out of this app, you want to ensure you have enabled it's settings correctly.

1. Open start menu
2. Type `Windows Security`
3. Open the `Windows Security App`

![image](https://user-images.githubusercontent.com/85346345/175436120-9ae59410-b0f4-4b24-a0c5-edd432c1a780.png)

Navigate through the menus and enable the following settings:

- Virus and Threat Protection
    - Real-Time Protection -> ON
    - Cloud-Delivered Protection -> ON
    - Tamper Protection -> ON
    - Controlled Folder Access^ -> ON

> ^Controlled folder access is a powerful tool to prevent damage caused by Ransomware, it will protect your personal files and folders in My Documents and other locations from unauthorized changes.

- Firewall & Network Protection
    - Firewall -> ON (for all three network types)

- App & Browser Control
    - Reputation-Based Protection
        - Check apps and files -> ON
        - Smartscreen for Microsoft Edge -> ON
        - Potentially unwanted app blocking -> ON
        - Smartscreen for Microsoft Store apps -> ON

- Device Security
    - Core Isolation
        - Memory Integrity -> ON (This can have a small performance impact on gaming)

### 2.4 Remove Unecessary Applications

Windows comes preinstalled with a large number of common applications, each extra application on a computer is more potential vulnerabilities to be exploited, A good rule of thumb is to only keep the apps installed that you need.

To remove apps easily:
1. Open Start menu
2. Type `Remove Apps`
3. Click `Add or Remove Programs`
4. Read Through the list of apps and remove anything that you do not frequently use.

### 2.5 Configure UAC to Maximum

UAC or User Account Control is a system in windows designed to help you prevent apps from making administrative changes without your awareness. UAC will prompt you to confirm whenever an application is trying to start or execute tasks that require administrator rights.

1. Open Start Menu
2. Type `UAC`
3. Select `Change User Account Control Settings`
4. Set the settings to "Always Notify"
5. Click `OK`

## 3 Network Security

These rules apply to your home network, they are common issues and flaws people often miss when setting up home routers and other equipment.

### 3.1 Change your Modem/Router Password

Your home router likely came with a default username and password, for many devices, these are exactly the same eg: username/password or admin/password. This is a critical security flaw as many people do not know how to change this password or don't bother.

If someone was able to enter your home network, via malware or a bad wifi password, they can potentially infect your Router device with malware or simply create more openings and vulnerabilities to your home network.

You should change your router password to something unique and complex.

1. Find out your Router/Modem Model (usually on a sticker on the device)
2. Google the user manual for your Router/Modem
3. Follow the manual to login tto your Router/Modem
4. Change the Router/Modem Administrator Password

Most routers/modems will also come with a guide in the box on how to login and chaneg settings on the router/modem.

If you have a seperate Wireless Access Point device, you should also ensure you change the default password on this device too, using similar steps to that above.

