<img align="center" src="/images/PIE-Logo.png" width="125px" alt="PIE">

    Phishing Intelligence Engine
    LogRhythm Security Operations
    v2.0  --  August, 2018

Copyright 2018 LogRhythm Inc. - See licensing details below

## [About]
    
![Phishing Intelligence Engine](/images/PIE.png)

The Phishing Intelligence Engine (PIE) is a framework that will assist with the detection and response to phishing attacks. An Active Defense framework built around Office 365, that continuously evaluates Message Trace logs for malicious contents, and dynamically responds as threats are identified or emails are reported.

##### :rotating_light: This framework is not officially supported by LogRhythm - use at your own risk! :rotating_light:

#### Features:

    - Analyze subjects, senders, and recipients using RegEx and Threat Feed correlation, to determine email risk.
    - Automatically respond to attacks by quarantining mail, blocking senders, and checking for clicks.
    - Sandbox analytics on all flagged email attachments and links.
    - Dynamic Case Management integration and metrics tracking.
    - Prevent sensitive data loss and verify corporate email security.


## [Additional Information]

Blog Post: https://logrhythm.com/blog/phishing-intelligence-engine-open-source-release/

BSides Vancouver 2018 Slides and Video: https://www.slideshare.net/heinzarelli/pie-bsides-vancouver-2018

BlueHat v17 Slides: https://www.slideshare.net/heinzarelli/phishing-intelligence-engine-bluehat-v17

Black Hat 2017 Slides: https://www.slideshare.net/heinzarelli/security-automation-and-orchestration

Security Weekly Webcast: https://www.youtube.com/watch?v=2oGMoGr4qBI 


## [Install and Usage]

Installation Walkthrough: https://www.youtube.com/watch?v=19bHJL0g154&feature=youtu.be

Configuration Guide (LogRhythm Community Access Required): https://community.logrhythm.com/t5/SIEM-articles/Phishing-Intelligence-Engine-PIE-Configuration-Guide/ta-p/39931

There are multiple aspects of this framework that all work together to detect and respond to Phishing attacks:

#### 1) [PIE Message Trace Logging](/Scripts/PIE_Message-Trace-Logging/)

The core of the Phishing Intelligence Engine - provides ongoing logging via the API, third party tool integrations, and automated email response.

#### 2) [Office 365 Ninja](/Scripts/O365-Ninja/)

The response arm of PIE. Quarantine mail, block senders, change credentials, check Office 365 configurations, and more.

#### 3) [SPAM Tracker](/Scripts/Spam-Tracker/)

List updater for ongoing tracking of spammer email addresses.

#### 4) [LogRhythm SIEM Dashboards](/SIEM-Dashboards/)

Analyst and Investigation Dashboards, which allow for searching and aggregation of Office 365 Data within the LogRhythm SIEM.

#### 5) [Alarms and Threat Lists](Alarms_and_Threat-Lists)

LogRhythm AIE alarm configurations and Threat List integrations.

#### 6) [LogRhythm SmartResponse](/SmartResponse/)
    
Plugins that can be integrated with the LogRhythm SIEM, allowing for automated response to alarms.

#### 7) [Report Phishing Message Button](/Outlook-Button/)

Addon for Microsoft Outlook to allow for easy reporting of Phishing Attacks.

#### 8) [Architecture](/images/PIE-Architecture.png)

High level overview of the PIE architecture and workflow:

![PIE Architecture](/images/PIE-Architecture.png)


## [Thanks!]

This project would not be a success without the folks below and the various third-party API integration providers. Thank you!

- [Jtekt](https://github.com/Jtekt) - Shodan Plugin, O365 Safelinks, bug fixes, and LR 7.3 API integration
- robert waight - LogRhythm Documentation, automated mailbox auditing, and various bug fixes
- bruce deakyne -  Cisco AMP Threat GRID Plugin
- jake reynolds - OpenDNS Plugin
- julian crowley - Message Tracking Log Parsing
- matt willems - LogRhythm Case API Plugin
- shaunessy o'brien - PIE Logo
- steve warburton - User Acceptance Testing
- zack rowland - Outlook Button
- SwiftOnSecurity - Phishing RegEx


## [Lead Author]

[Greg Foss](https://github.com/gfoss) - formerly of LogRhythm Labs


## [License]

Copyright 2018 LogRhythm Inc.   

PowerShell code is Licensed under the MIT License. See LICENSE file in the project root for full license information.

LogRhythm integrated code (SmartResponse and Dashboards) is licensed pursuant to the LogRhythm End User License Agreement located at https://logrhythm.com/about/logrhythm-terms-and-conditions/ (“License Agreement”) and by downloading and using this content you agree to the terms and conditions of the License Agreement unless you have a separate signed end user license agreement with LogRhythm in which case that signed agreement shall govern your licensed use of this content. For purposes of the applicable end user license agreement, this content constitutes LogRhythm Software
