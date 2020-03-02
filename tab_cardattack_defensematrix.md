---

title: tab_cardattack_defensematrix
displaytext: Card Attack / Defense Matrix
layout:  null
tab: true
order: 1
tags: top 10 card game

---

## Card Attack / Defense Matrix


| Attacks| TA Playing Card| Threat Agent (TA) Point of View| Proactive DC| DC Playing Card| Defense Control (DC) Concepts|
|------------|------------|------------------------|------------|------------|------------------------|
|A1|Ace|Injection – TAs send simple text based data as part of a command or query that exploits the syntax rules of the targeted system’s interpreter. Many DC teams continue to allow the use of unsafe APIs and are lax in reviewing legacy code for injection flaws, keeping data separate from commands and limiting SQL injection mass disclosures.|C3|3|Secure Database Access - Untrusted data and input is properly controlled and handled by database and platform authentication and communication controls.|
|A1|Ace|Injection – TAs send simple text based data as part of a command or query that exploits the syntax rules of the targeted system’s interpreter. Many DC teams continue to allow the use unsafe APIs and are lax in reviewing legacy code for injection flaws, keeping data separate from commands and limiting SQL injection mass disclosures.|C4|4|Encode and Escape Data - Applications are designed to encode and escape data to ensure that TA crafted scripts are prevented from hijacking the intended process.|
A2|2|Broken Authentication – System flaws allow TAs to compromise passwords, keys, or session tokens, or to assume other users’ identities. Privileged accounts are frequently targeted. The prevalence of broken authentication is widespread across the DC landscape due to poor design and weak implementation of identity and access controls. Effective reconnaissance will help identify systems that may be using admin default credentials.|C6|6|Implement Digital Identity - Properly configured user authentication and session management controls are in place to ensure that only legitimate users and processes are permitted.|
A3|3|Sensitive Data Exposure – TAs steal clear text data off the server, while in transit, or from the users browser. Over the last few years, this attack has seen successful TA exploits. DC teams are not ensuring that business sensitive data is encrypted. Sensitive data maybe stored or cached long after it is needed for any business purpose. When crypto is employed, weak key generation and management, and weak algorithm, protocol and cipher usage is common, particularly for weak password hashing storage techniques. For data in transit, server side weaknesses are mainly easy to detect, but hard for data at rest.|C8|8|Protect Data Everywhere - A process is in place to ensure that sensitive user; platform and application data is properly classified, encrypted and controlled.|
A4|4|XML External Entities (XXE) - TAs upload hostile content to XML processors or documents. DC management continues to disregard this risk and frequently fails to support funding for Web Application Firewalls, XXE testing and essential developer training to identify and mitigate XXE.|C4|4|Encode and Escape Data - Applications are designed to encode and escape data to ensure that TA crafted scripts are prevented from hijacking the intended process.|
A5|5|Broken Access Control – TAs know that flawed applications and APIs may allow users to move beyond management’s intended permissions. Access control weaknesses are common due to the lack of automated detection and effective functional testing by application developers.|C7|7|Enforce Access Controls - Steps have been taken to ensure that user roles are properly managed and that need-to-know and data sensitivity access controls are properly configured.|
A6|6|Security Misconfiguration – TAs exploit unpatched flaws or access default accounts, unused pages, unprotected files and directories to gain unauthorized access or knowledge of the system. Without a robust and mature DC process, it is virtually impossible for companies to properly harden all assets resulting in application stack security misconfigurations permitting successful exploits of network services, platforms, web servers, application servers, databases, frameworks, custom code, and pre-installed virtual machines, containers, or storage.|C1|Ace|Define Security Requirements - Standardized security requirements are in place and supported by adequate resources to ensure that assets are properly secured, configured, patched and upgraded.|
A7|7|Cross-Site Scripting (XSS) – TA input is not prevented from updating a web page with malicious data resulting in hijacked user sessions, defaced web sites, redirected users and malware. DC teams are not following the OWASP XSS Prevention Cheat Sheet and TAs around the globe are leveraging this risk. It is found in approximately two-thirds of all applications.|C4|4|Encode and Escape Data - Applications are designed to encode and escape data to ensure that TA crafted scripts are prevented from hijacking the intended process.|
A8|8|Insecure Deserialization – TAs exploit weaknesses in applications and APIs that permit the deserialization of hostile TA data. TA exploitation of deserialization is difficult, as off the shelf exploits rarely work without changes or tweaks to the underlying exploit code.|C5|5|Validate All Inputs - Processing controls are in place to prevent the server-side handling of invalid input and design controls are in place to minimize the use of serialized data formats.|
A9|9|Known Vulnerabilities - TAs identify weak components through scanning or manual analysis and customize attack exploits. Prevalence of this issue in the business community is widespread. Component-heavy development patterns has resulted in development teams not understanding which components they use in their application or API, much less keeping them up to date. DC teams may be limited in their efforts to scan, identify and remove unnecessary functions and monitor libraries.|C2|2|Leverage Security Frameworks and Libraries - Only trusted frameworks and libraries with solid security features are employed.|
Black Hat|Joker|Phishing attack – Phishing controls include day-to-day procedures and education and are rarely designed with the holistic view necessary to mount an effective defense. There are few DC precautions that application writers can follow to reduce this risk. DC and business management have historically been lax in addressing phishing controls.|None||User Education - Effective DC actions to blunt a phishing attack are limited.|
A10|10|Logging & Monitoring - TAs rely on ineffective application runtime security logging, inconsistent operational data reviews, and the poor overall management of monitoring activities, coupled with weak responses by the DC team, to achieve their goals without being detected. This card represents additional malware that supports the attack card (A1 through A9). It is used during the attack phase. It is not a stand-alone attack card. The A10 card may be added to support the TA’s attack card during the current or subsequent attack rounds. The A10 card may only be played during an Assess Web Platform Technical Weaknesses Attack or PWN Attack. The TA’s A10 card may be any color.|
||||C9|9|Logging and Monitoring - This card represents the effective logging and monitoring of the web platform’s operational data and application’s processing activities.
||||||
||||||The C9 Logging and Monitoring DC card cancels TA attacks (1 through 9) unless the attack vector path (1, 2 or 3) is poisoned by the A10 malware card.
||||||
||||||The C9 card may be any color.
||||||
||||||The C9 defense is not effective if the TA attacking site is masked.
||||||
||||||The C9 card can only be played during the Assess Web Platform Technical Weaknesses Attack and the PWN Attack.
|||White Hat|C10|10|Error and Exception Handling - With this card, controls are in place to ensure that the application’s error and exception handling process does not leak system information and that it is guarded from malicious system overload.
||||||
||||||The C10 card may be any color.
||||||
||||||The C10 Error Handling DC card cancels TA attacks (1 through 9) unless the DC’s face card attack vector path (1, 2 or 3) is poisoned by the A10 malware card.
||||||
||||||The C10 card can only be played during the Assess Web Platform Technical Weaknesses Attack and the PWN Attack.
|||||Joker|DC White Hat Joker - The DC White Hat Joker card can be played any time while under attack to prevent a phishing attack or a pivot move in the assigned vector path. Once in play, the DC White Hat Joker card cannot be moved from the assigned position.

|Special Attack and Defense Rules|
|----------------------------------------------------------------------------------------------------------|
|Observation Attack - If the TA site is not masked, the color of TA’s attacking card (A1 through A9) must match the color (red or black) of the TA’s attack site card. For example, an attacking unmasked TA Queen of Hearts (Red) may only use a Red (Diamond or Heart) attack (A1 through A9) card.|
|Assess Web Platform Technical Weaknesses Attack - If the TA site is not masked, the suit of the TA’s attacking card (A1 through A9) must match the suit (hearts, diamonds, spades, or clubs) of the defending DC site card.|
|PWN Attack - If the TA site is not masked, the attacking TA site (Queen or King) must match the face card (Queen or King) of the defending DC site card. An unmasked Jack may still attack any other face card. For example, an attacking unmasked TA Queen of Hearts may only launch a PWN attack against a DC Queen (Hearts, Diamond, Club or Spades).|

