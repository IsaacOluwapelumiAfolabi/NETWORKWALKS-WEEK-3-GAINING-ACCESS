# Week 3 – Gaining Access: Password Cracking

**Cybersecurity & Ethical Hacking Internship | NetworkWalks**  
**Author:** Isaac Afolabi  
**Week:** 03  
**Focus:** The third stage of the cyberattack lifecycle – Gaining Access

## Overview

This repository documents two authorized training exercises involving password recovery from a training-provided, password-protected PDF file (`My Locked PDF1.pdf`).

The exercises covered PDF hash extraction, password auditing/recovery workflows, and the security risks of weak or reused passwords.

> **Authorization and safety:** These techniques were used only on the PDF supplied for the assigned training exercise. Do not use password-cracking tools against files, accounts, or systems without explicit permission.

## Learning objectives

- Understand the relationship between protected files, password hashes, and password recovery.
- Gain familiarity with John the Ripper and its Johnny graphical interface.
- Practice the hash extraction and recovery workflow using NetworkWalks tools.
- Understand why strong, unique passwords and multi-factor authentication matter.

## Project modules

### Project Module 1 – John the Ripper (JTR) and Johnny GUI

**Objective:** Recover the password of the assigned PDF using John the Ripper and Johnny GUI on Windows.

**Tools used:**
- Windows PC
- Online Hash Crack – PDF hash extraction
- John the Ripper (JTR)
- Johnny GUI

**Workflow performed:**
1. Installed John the Ripper and Johnny GUI.
2. Used Online Hash Crack to extract the hash from the training PDF.
3. Saved the extracted hash in a text file.
4. Loaded the hash file into Johnny GUI.
5. Started the password-recovery process.
6. Confirmed the successful result in Johnny GUI.

**Observed result:** Johnny GUI reported `1 cracked, 0 left` for the PDF hash. The recovered password and extracted hash have intentionally been removed from the public evidence.

See [`Project-Module-1-JTR-Johnny/README.md`](Project-Module-1-JTR-Johnny/README.md).

### Project Module 2 – NetworkWalks Hash Calculator and Password Cracker

**Objective:** Recover the password of the assigned PDF using NetworkWalks' web-based tools.

**Tools used:**
- NetworkWalks Hash Calculator: https://networkwalks.com/hash-calculator/
- NetworkWalks Password Cracker: https://networkwalks.com/password-cracker/
- Windows laptop and web browser

**Workflow performed:**
1. Opened the NetworkWalks Hash Calculator.
2. Uploaded the assigned PDF and extracted its hash.
3. Copied the hash output.
4. Opened the NetworkWalks Password Cracker.
5. Submitted the hash and started the recovery process.
6. Completed the exercise and captured the platform's completion confirmations.

See [`Project-Module-2-NetworkWalks/README.md`](Project-Module-2-NetworkWalks/README.md).

## Key takeaways

- Use long, strong, unique passwords for every account.
- Avoid password reuse because a credential exposed on one service may be tried elsewhere.
- Enable multi-factor authentication (MFA).
- Use a reputable password manager to create and store unique passwords.
- Protect password hashes and sensitive files from unauthorized access.
- Perform password audits only within an approved scope.

## Repository structure

```text
WEEK-3-GAINING-ACCESS-REPOSITORY/
├── README.md
├── Project-Module-1-JTR-Johnny/
│   ├── README.md
│   └── Evidence/
├── Project-Module-2-NetworkWalks/
│   ├── README.md
│   └── Evidence/
└── Learning-Outcomes/
    └── Key-Lessons.md
```

## Evidence handling

Screenshots are included as supporting evidence. Password values, extracted hash material, and individual training flag strings have been redacted to avoid publishing sensitive or challenge-specific information in a public repository.

## Disclaimer

This repository is for educational and portfolio documentation. All practical work was limited to the assigned training file and authorized lab environment.
