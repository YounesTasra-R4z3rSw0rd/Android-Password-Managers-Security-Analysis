<h1 align="center">
  <br>
    🔎 Android Password Managers Security Analysis 🔍
  <br>
  <br>
</h1>

<h4 align="center">Static & Dynamic Analysis of the 5 most popular password managers on Android</h4>
<h4 align="center">Keeper, NordPass, LastPass, Bitwarden, and 1Password</h4>
<p align="center">
  <a href="https://twitter.com/YounesTasra"><img src="https://img.shields.io/badge/twitter-%40YounesTasra-blue.svg" alt="@YounesTasra" height="18"></a>
  <a href="https://www.linkedin.com/in/younes-tasra-95a1a4234/"><img src="https://img.shields.io/badge/linkedin-%40YounesTasra-blue.svg" alt="younes-tasra-95a1a4234" height="18"></a>
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" height="18"></a>
</p>
<br>

## Abstract
Cybersecurity has become one of the most important and constantly evolving areas in the IT and technology industry. Faulty security has resulted in immense losses to the global economy. Oftentimes, the pitfall in such financial loss is due to the security of passwords, since they are considered the first line of defense against cyber threats. This is the reason why it is important to create and store strong and secure passwords. Password managers allow the storage and retrieval of sensitive information from an encrypted database. Users rely on them to provide better security guarantees against trivial exfiltration than alternative ways of storing passwords, such as an unsecured flat text file.
The purpose of this project is to decompile and analyse five popular password managers on Android platform: `Keeper`, `NordPass`, `LastPass`, `Bitwarden` and `1Password`. The analysis includes both `static` and `dynamic` methods to evaluate the security of the master password and the derived keys. The report provides detailed information about each password manager, including the methodology used for the analysis, the vulnerabilities identified, and the potential impact on user security.

## Methodology
The analysis used a combination of static and dynamic methods to evaluate the security of the password managers. 
* `Static analysis` involved examining the source code of each password manager to identify any vulnerabilities. 
* `Dynamic analysis` involved running each password manager on an Android emulator and monitoring the network traffic to identify any potential security issues.

## Password Managers Analyzed
The following password managers were analyzed in this report:
* [Keeper](https://www.keepersecurity.com/)
* [NordPass](https://nordpass.com/homepage/)
* [LastPass](https://www.lastpass.com/)
* [Bitwarden](https://bitwarden.com/)
* [1Password](https://1password.com/)

## Tools & Environment
The following tools and environment were used for the analysis:
* [Genymotion](https://www.genymotion.com/): to run the Android emulator for dynamic analysis
* [Apktool](https://ibotpeaches.github.io/Apktool/): to decompile the APK files
* [ADB](https://developer.android.com/studio/command-line/adb): to install the APK files on the emulator and extract data from the devices
* [Dex2Jar](https://github.com/pxb1988/dex2jar): to convert the DEX files to JAR files for static analysis
* [Burpsuite](https://portswigger.net/burp): to intercept and analyze network traffic during dynamic analysis
* [Jadx](https://github.com/skylot/jadx): to decompile the JAR files for static analysis
* [OpenSSL](https://www.openssl.org/): to generate and manage cryptographic keys for analysis
* [Objection](https://github.com/sensepost/objection): to perform runtime manipulation of the password managers during dynamic analysis
* [Frida](https://frida.re/docs/home/):  to perform dynamic analysis on the password managers

## Report
The [full report](https://raw.githubusercontent.com/YounesTasra-R4z3rSw0rd/Android-Password-Managers-Security-Analysis/main/Password%20Managers%20Security%20Analysis.pdf) is available in the PDF file located in this repository. The report contains detailed information about each password manager, the methodology used for the analysis, the vulnerabilities identified, and recommendations for improving security.

## Disclaimer
The purpose of this analysis is to identify potential security issues with password managers on the Android platform. This analysis is not intended to be a comprehensive review of each password manager's security features, and the results should not be used as the sole basis for selecting a password manager. Users should always exercise caution when using any password manager and take additional security measures, such as enabling two-factor authentication, to protect their accounts.

## License
This project is licensed under the MIT License - see the [License](https://github.com/YounesTasra-R4z3rSw0rd/Android-Password-Managers-Security-Analysis/blob/main/LICENSE) file for details.
