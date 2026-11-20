# PENETRATION TESTING REPORT
### GAINING ACCESS – PASSWORD CRACKING

**W3-PM-FINAL  |  CYBERSECURITY  |  NETWORKWALKS**

| Field | Detail |
|---|---|
| **Pentester Name (Cybersecurity Professional)** | **Isaac Afolabi** |
| **Program/Batch** | B084-Networkwalks |
| **Date** | 20 November 2026 |
| **Modules completed** | W3-PM1 – PDF Password Cracking with John the Ripper and Johnny GUI W3-PM2 – PDF Password Cracking with NetworkWalks Tools|
| **Client/Target** |Training-provided password-protected PDF|
| **Permission / Scope** | Assigned educational lab exercise; testing limited to the supplied PDF file|
| **Phases covered** | **Phase 3:**  Gaining Access – password recovery exercise<br> |

# 1. Liability Disclaimer

I performed these activities as part of an assigned cybersecurity training exercise and limited the work to the password-protected PDF supplied for the lab. Password recovery and hash-cracking techniques should only be used on files and systems that the tester owns or is explicitly authorized to assess. This report is for educational purposes and does not authorize access to any other file, account, device or system.

# 2. Introduction

This report documents my Week 3 practical activities on the third stage of the cyberattack lifecycle: Gaining Access. The focus was password cracking and password recovery using a supplied password-protected PDF file named My Locked PDF1.pdf.

I completed two project modules. In Module 1, I extracted the PDF hash using Online Hash Crack and used John the Ripper through the Johnny graphical interface to recover the password. In Module 2, I used the NetworkWalks Hash Calculator and Password Cracker. I successfully recovered the PDF password during the exercises.

The exercises helped me understand how password-protected files can be assessed through hash extraction and password-recovery tools, and why strong, unique passwords are important.


# 3. Tools Used

The table below lists each tool used in this report and its purpose.

| Tool | Purpose |
|---|---|
| Windows PC | Operating systems used for reconnaissance activities             |
| Online Hash Crack               | Find domain registration details (owner, dates, name servers).   |
| John the Ripper (JTR)              | Fingerprint web technologies (server, CMS, plugins, IP).         |
| Johnny GUI              | Resolve the domain name to its IP address using DNS.             |
| NetworkWalks Hash Calculator              | Read the HTTP response headers of the website.                   |
| NetworkWalks Password Cracker             | Detect whether a Web Application Firewall protects the site.     |


# 4. Activities Performed

## 4.1 Project Module 1 – PDF Password Cracking with John the Ripper and Johnny GUI

**Objective:** Recover the password of the assigned PDF using John the Ripper and its Johnny graphical interface.

**Procedure:** I downloaded and installed John the Ripper and Johnny GUI on my Windows PC. I then used Online Hash Crack to extract the hash from My Locked PDF1.pdf. I copied the extracted hash into a text file, loaded that file into Johnny GUI, and initiated the password-recovery process.

**Result:** Johnny GUI displayed the recovered password as `**good-luck**` and showed **100%** (1/1: 1 cracked, 0 left) for
the PDF format. I then attempted to open the protected PDF using the recovered password.

## 4.2 Project Module 2 – PDF Password Cracking with NetworkWalks Tools

**Objective:** Use the NetworkWalks Hash Calculator and Password Cracker to recover the password of the assigned
PDF.

**Procedure:** I opened the NetworkWalks Hash Calculator in a web browser, uploaded the PDF and extracted its hash. I copied the hash value, opened the NetworkWalks Password Cracker, pasted the hash into the tool and started the password-cracking process. The tools used for this module were the NetworkWalks Hash Calculator `(networkwalks.com/hash-calculator)` and the NetworkWalks Password Cracker `(networkwalks.com/password-cracker)`.

**Result:** I successfully completed the password-recovery exercise and captured the completion flags displayed by the
training platform.

# 5. Results and Evidence Summary

| **\#** | **Module**                           | **Observed Result**                                  | **Status**                                                                                            |
|--------|----------------------------------------------|-------------------------------------------------------------|-----------------------------------------------------|
| 1      | Module 1 – JTR / Johnny          | Johnny GUI reported 1 of 1 PDF hashes cracked and displayed the recovered password as good-luck       | Completed |
| 2      | Module 2 – NetworkWalks          | The password-cracking exercise was completed and three training completion flags were captured in the supplied screenshots.      | Completed |

# 6. Risk Analysis / Impact

| **\#** | **Risk / Finding**                           | **Evidence / Observation**                                  | **Potential Impact**                                                                                            | **Risk Level** |
|--------|----------------------------------------------|-------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|----------------|
| 1      | Weak or predictable password                 |The lab PDF password was recovered during the exercise         | Weak passwords may be easier to recover,increasing the risk of unauthorized access to protected files.         | **● Medium**   |
| 2      | Password reuse                               | The learning exercise highlighted the danger of reusing passwords across accounts    | A password exposed on one service may be tried against other accounts.                | **● High**      |
| 3      | Exposure of password hashes                  | The PDF hash was extracted for password-recovery testing.     | If hashes are exposed, attackers may attempt offline password guessing or cracking.                      | **● Medium**      |

**Risk level key:** ● Critical ● Medium ● Low

Risk levels above are general assessments of the security implications of the demonstrated techniques. They are not findings of a compromise or vulnerability in an external organization or production system.

# 7. Recommendations

Based on the lessons from these exercises, I recommend the following security practices:

**1. Use strong, unique passwords.** Create long passwords or passphrases that are difficult to guess and avoid
using the same password across multiple accounts.

**2. Enable multi-factor authentication.** Add another verification factor to important accounts so that a compromised
password alone is less likely to provide access.

**3. Use a reputable password manager.** A password manager can help generate and store unique passwords
securely.

**4. Protect password hashes and sensitive files.** Limit access to stored credentials and protected documents, and
use secure storage and appropriate encryption.

**5. Apply secure password storage practices.** For applications, store passwords using a purpose-built
password-hashing algorithm with unique salts and suitable work factors rather than reversible encryption or fast
general-purpose hashes.

**6. Conduct authorized password audits.** Organizations should periodically assess password strength within a
clearly approved scope and handle recovered credentials securely.

# 8. Conclusion

During Week 3 of my Cybersecurity and Ethical Hacking internship, I studied the Gaining Access stage of the cyberattack lifecycle, focusing on password cracking and password security.

I completed two practical modules. In Module 1, I used Online Hash Crack to extract a PDF hash and John the Ripper through Johnny GUI to recover the password. The Johnny interface reported that one out of one PDF hashes had been cracked and displayed the recovered password. In Module 2, I used the NetworkWalks Hash Calculator and Password Cracker and successfully completed the exercise, capturing the training platform's completion flags.

These activities improved my understanding of hash extraction, password-recovery tools, and the risks associated with weak or reused passwords. I also learned that password cracking tools can be used by security professionals for authorized password auditing and awareness training.

All practical activities documented in this report were limited to the assigned training exercise and the supplied PDF
file.

# 9. Evidences Collected

The following screenshots are included as supporting evidence for the activities described in this report.
*Screenshots collected as evidence during the activities (stored in the `screenshots/` folder):*

## Evidence 1 – PDF hash extraction using Online Hash Crack

### Evidence 1 – PDF hash extraction using Online Hash Crack
![NSLOOKUP Result](NSLOOKUPRESULT.png)

### Evidence 2 – Johnny GUI showing the recovered password and 1/1 cracked result
![Topology Saveshot](TOPOLOGYSAVESHOT.PNG)

### Evidence 3 – Password-protected PDF opening prompt
![WAWOOF Result](WAWOOFRESULT.png)

### Evidence 4 – NetworkWalks training completion flag
![WhatWeb Result](WHATWEBRESULT.png)

### Evidence 5 – NetworkWalks JTR-related completion flag
![WHOIS Result 1](WHOISRESULT1.png)
![WHOIS Result 2](WHOISRESULT2.png)

### Evidence 6 – Additional NetworkWalks completion flag
![DNSRecon Result](dnsreconresult.png)



-End-
