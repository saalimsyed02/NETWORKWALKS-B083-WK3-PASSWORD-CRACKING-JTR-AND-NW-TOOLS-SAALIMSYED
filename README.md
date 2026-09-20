# Week 3 Internship Project: Password Cracking Modules

## Overview
This repository contains the completed project tasks for Week 3 Cybersecurity & Ethical Hacking Internship focusing on password cracking methodologies. The project covers two main modules performed across multiple target files (`PDF 1`, `PDF 2`, and `PDF 3`):
1. **Project Module 1:** Password Cracking using **John the Ripper (CLI)** and **Johnny (GUI)** on Windows.
2. **Project Module 2:** Password Cracking using **Networkwalks Hash Calculator & Password Cracker** browser tools.

---

## Project Module 1: Password Cracking with JTR (John the Ripper & Johnny)

### Objective
Recover the passwords of encrypted PDF files (`PDF 1`, `PDF 2`, and `PDF 3`) using offline desktop tools (John the Ripper and Johnny GUI).

### Step-by-Step Implementation & Evidence

* **Step 1: Tool Installation and Setup**
  Downloaded John the Ripper (JTR Jumbo) and installed the Johnny GUI interface, linking `john.exe` within Johnny's settings.
  <img width="1916" height="955" alt="Screenshot 2026-09-20 163452" src="https://github.com/user-attachments/assets/831ea77d-1f19-47de-b7f3-02864a716778" />

  > *Figure 1.1: Johnny configured with the path to `john.exe`.*

* **Step 2: Hash Extraction**
  Used an online extraction utility to extract secure hash values from the locked PDF files (`PDF 1`, `PDF 2`, and `PDF 3`).
  <img width="1705" height="851" alt="image" src="https://github.com/user-attachments/assets/747c9892-2ec0-45ed-b1db-db2840084aaf" />

  > *Figure 1.2: Extracted PDF hash starting with `$pdf$`.*

* **Step 3: Saving the Hash Files**
  Created text files (`hash1.txt`, `hash2.txt`, and `hash3.txt`) using Notepad and saved each extracted hash string securely.
  <img width="1912" height="877" alt="image" src="https://github.com/user-attachments/assets/2148e6a8-2575-46fc-a0b6-108b7be01f44" />

  > *Figure 1.3: Hashes saved individually in text files.*

* **Step 4: Running the Attacks in Johnny**
  Loaded each hash file sequentially into Johnny and executed password cracking sessions for `PDF 1`, `PDF 2`, and `PDF 3`.
  > <img width="1907" height="992" alt="Screenshot 2026-09-20 164744" src="https://github.com/user-attachments/assets/bdcea013-b7b7-4f2f-8315-8c18993051de" />
  <img width="1916" height="1007" alt="image" src="https://github.com/user-attachments/assets/9ec0b4ca-f600-451e-894f-ca6c506e3093" />

  > *Figure 1.4: Passwords successfully cracked in Johnny for all PDF targets.*

* **Step 5: Unlocking the PDFs**
  Opened the encrypted PDF files (`PDF 1`, `PDF 2`, and `PDF 3`) using their respective recovered plain-text passwords to capture the completion flags.
  <img width="591" height="443" alt="Screenshot 2026-09-20 185704" src="https://github.com/user-attachments/assets/c0ad0264-c23a-4569-a787-3e4ec44c8472" />
  <img width="1886" height="945" alt="Screenshot 2026-09-20 165052" src="https://github.com/user-attachments/assets/6b8a28f5-45ff-4231-8457-9ee71aaf8fae" />

  > *Figure 1.5: Successful decryption and flag captures across all files.*

---

## Project Module 2: Password Cracking with Networkwalks Tools

### Objective
Perform web-based hash extraction and dictionary-based password cracking using the specialized browser tools provided by Networkwalks across all target PDF files (`PDF 1`, `PDF 2`, and `PDF 3`).

### Step-by-Step Implementation & Evidence

* **Step 1: Hash Calculation / Extraction**
  Navigated to the Networkwalks Hash Calculator tool and uploaded each locked PDF (`PDF 1`, `PDF 2`, and `PDF 3`) to generate their respective crackable hash formats (`$pdf$`).
  <img width="1226" height="813" alt="Screenshot 2026-09-20 184601" src="https://github.com/user-attachments/assets/56c71264-4411-40a6-a2a7-8f729c51a424" />

  > *Figure 2.1: PDFs uploaded and hashes generated via Hash Calculator.*

* **Step 2: Password Cracker Dictionary Attack**
  Copied the full hash values, pasted them into the Networkwalks Password Cracker tool, and initiated built-in dictionary attacks for each file.
 
* **Step 3: Successful Password Recovery**
  The tool matched the hashes against the dictionary lists and successfully retrieved the plain-text passwords for all three files.
 

* **Step 4: Final Document Unlocking**
  Inputted the recovered passwords into the PDF reader to unlock each secure document (`PDF 1`, `PDF 2`, and `PDF 3`) and verify the completion milestones.
 
---

## Key Learnings & Security Takeaways
* **Hashing vs. Encryption:** Encryption is a two-way reversible function requiring a decryption key, whereas hashing is a one-way mathematical function used for validation.
* **Password Strength Importance:** Simple and short passwords can be cracked within minutes via dictionary or brute-force attacks across multiple files, underscoring the critical need for complex, long passphrases.
