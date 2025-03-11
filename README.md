# Em's simple guide for cyber security

These are a handfull of simple and easy recommendations that I have pulled together over the years to improve your home security on a windows PC and help you feel confident and safe online.

> Background: I have been working in the IT Industry for over 7 years, covering roles from Helpdesk support, Network Engineering and more recently Cloud Security and consulting. As such I have worked on a wide variety of platforms, applications and tools. This guide is a collection of some of the basic recommendations which I would make to anyone who wants to have a bit more control over their own personal security and their online footprint.

NOTE: This is a work-in-progress and I will be adding more content to this over time. If you see any errors or mistakes, please feel free to create a PR or contact me directly. My details are in my Bio.

> Furthermore, if you are looking for some more advanced recommendations, be sure to check out the [Advanced Guides](https://github.com/CMDRMgram/BasicSecurityManual/tree/main/Advanced%20Guides) folder. I will be periodically adding new guides and recommendations here individually.

## 1 Account Management

### 1.1 Use a Password Manager (Paid/Free)

Re-using passwords is a very quick way to have all your accounts hacked, If so much as one service is breached you might find yourself in a lot of trouble very quickly. I strongly recommend using a password manager, to store passwords and ensure you create unique passwords for every service.

Here are some I recommend:

- [Bitwarden](https://bitwarden.com/) (Cloud Service, Free, Offline Option available)
- [KeePass](https://keepass.info) (Stored on your PC, Free)

DO NOT keep passwords in a text file/word document/etc on your PC, this is the first thing potential hackers will look for.

### 1.2 Use Good Passwords

Good passwords are suprisingly hard to come by, but they don't need to be difficult. Here is a very simple formula for creating complex and memorable passwords.

- a few words
- a few symbol between the words
- some words in all CAPS
- 2 numbers at the end

Examples:

- summer-CAKES88
- GREEN@clouds44
- bright!GLASS23

[A well known XKCD comic explains how these work in detail.](https://xkcd.com/936/)

These passwords will meet 99% of requirements and are easy to remember.

DO NOT:
- Use sequential passwords (password1, password2)
- Use dates or birthdays
- Use names of people you know personally

> [!NOTE]  
> If you are using a password manager, you should use long randomly generated passwords (20+ Characters) and store these in the password manager. Create a good memorable password to unlock the password manager.

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

> Your recovery keys are sacred, these should be kept offline and secure. For example, print them out and keep them safely stored away somewhere secure at home. Do not label them. Alternatively, create an Encrypted USB drive, and store keys within it.

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
    - Controlled Folder Access -> ON

> Controlled folder access is a powerful tool to prevent damage caused by Ransomware, it will protect your personal files and folders in My Documents and other locations from unauthorized changes.

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
        - Memory Integrity -> ON

> Memory Integrity can have a small performance impact on gaming and other performance intensive tasks. Use as you feel comfortable.

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

### 2.6 Do not Daily-drive an Admin Account

When you first setup your computer, you were likely given an Administrator account, this allows you to install and setup apps and software easily without needing admin permissions. However, this also means that when you run applications, they may be running as an administrator with more access rights then they need. It also opens the possiblility to make dangerous changes to the system unintentionally.

Generally speaking, you should only be using an Administrator account when you need to make Administrative changes, otherwise you should be using a "Standard" account. 

This can be a little complex but it is a significant improvement to your computer security. 

Firstly, check to see if your account is an administrator

Windows 11 Steps: 

> Steps for windows 10 are very similar

1. Open `Settings`
2. Go to `Accounts > Other Users`
3. Check to see what type of account you are using under your username:
    - Administrator
    - Standard
  
If you are using an `Administrator` account, we will need to create a new Administrator User and demote your current account to `Standard`

Creating a new Administrator Account:

1. Open `Settings`
2. Go to `Accounts` > `Other Users`
3. Select `Add Account` under Other Users ![image](https://user-images.githubusercontent.com/85346345/175455345-cd84b0b1-a2c7-42d1-8688-ada85a10b6e4.png)
4. Select `I don't have this person's sign-in information`
5. Select `Add a user without a Microsoft account` (This is for creating a local account)
6. Give the accounts a Username and a Strong Password (see [Section 1.2](https://github.com/CMDRMgram/BasicSecurityManual#12-use-good-passwords))
7. Setup some security questions
8. Select the New Account
9. Go to `Account Options` > `Change account type`
10. Change `Account type` to `Administrator` and click `OK`

Once complete, it should look something like this:

![image](https://user-images.githubusercontent.com/85346345/175455935-88067420-3af5-440f-b1b6-af39af23ed30.png)

Now finally, you need to demote your existing account.

1. Log into the new Administrator you created (Start Menu > Switch user > Select `Other User`)
2. Open `Settings`
3. Go to `Accounts` > `Other Users`
4. Select your Primary Account
9. Go to `Account Options` > `Change account type`
10. Change `Account type` to `Standard` and click `OK`

You can now switch back to your Primary Account.

> Once you have done this, when installing applications or changing settings, you may be prompted to enter Administrator details, you should keep your Admin Account login somewhere safe and secure, such as a Password manager as mentioned in [Section 1.1](https://github.com/CMDRMgram/BasicSecurityManual#11-use-a-password-manager-paidfree)

## 3 Network Security

These rules apply to your home network, they are common issues and flaws people often miss when setting up home routers and other equipment.

### 3.1 Change your Modem/Router Password

Your home router likely came with a default username and password, for many devices, these are exactly the same eg: username/password or admin/password. This is a critical security flaw as many people do not know how to change this password or don't bother.

If someone was able to enter your home network, via malware or a bad wifi password, they can potentially infect your Router device with malware or simply create more openings and vulnerabilities to your home network.

You should change your router password to something unique and complex.

1. Find out your Router/Modem Model (usually on a sticker on the device)
2. Google the user manual for your Router/Modem
3. Follow the manual to login to your Router/Modem
4. Change the Router/Modem Administrator Password

Most routers/modems will also come with a guide in the box on how to login and chaneg settings on the router/modem.

If you have a seperate Wireless Access Point device, you should also ensure you change the default password on this device too, using similar steps to that above.

## 4 Internet Security

### 4.1 VPNs

Im not going to do what most here and tell you that "you MUST be using a VPN to be safe on the internet" because frankly thats bullshit.

A VPN works by routing your internet traffic through a VPN server before spitting it back out into the internet, essentially a proxy server.

It is a common misconception that VPNs make your internet browser more "secure" because it's "encrypted"...

There are two major issues with this...
1. Your internet traffic is ALREADY ENCRYPTED from End-to-End, its called TLS and if you see "HTTPS://..." you are using it. See Image 
![image](https://user-images.githubusercontent.com/85346345/187901914-1180a41e-ab8b-40eb-8662-ab329387c6a3.png)
2. VPNs do add extra encryption, but it is ONLY from your computer to the VPN's server, it still has to travel across the internet after that without the "extra" encryption the VPN provides, which makes it functionally pointless.

VPNs (the consumer kind) are NOT giving you extra security, they are giving you privacy in the form of obscuring your location, nothing more.

Regarding privacy however, your location is not typically something advertisers will use anyway, since your IP changes regularly and you IP geolocation is usually only accurate to the city.

If you want to have ACTUAL privacy, you need to look into your browser privacy settings and how you use website and services, I will go into more detail on this further.
