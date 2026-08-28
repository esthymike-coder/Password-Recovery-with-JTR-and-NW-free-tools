# Password-Cracking-and-Security-Assessment-Lab

🔐 Password Cracking and Security Assessment Lab

Overview

This project documents a controlled cybersecurity laboratory exercise focused on password cracking, hash extraction, password recovery, and the security implications of weak passwords.

The project was completed as part of a cybersecurity and ethical hacking practical exercise and involved two complementary approaches to password recovery:

1. John the Ripper (JTR) and Johnny GUI
2. Networkwalks Hash Calculator and Password Cracker

The objective was to understand, in a controlled and authorized environment, how a password-protected PDF can be assessed by extracting its password hash and attempting to recover the original password.

The practical work was performed on a personal laboratory environment, and screenshots were captured throughout the process to document the procedures and results.

---

⚠️ Disclaimer

This repository documents an authorized cybersecurity laboratory exercise performed for educational and skill-development purposes.

All password-recovery activities were performed against the provided laboratory material. The techniques demonstrated in this repository should only be used on systems, files, or accounts for which explicit authorization has been granted.


---

🎯 Project Objectives

The primary objectives of this project were to:

- Understand the relationship between passwords, hashes, and password-protected files.
- Learn how password hashes can be extracted from protected documents.
- Use John the Ripper to perform a controlled password-recovery exercise.
- Explore the Johnny graphical interface for John the Ripper.
- Use Networkwalks security tools to extract and analyze a PDF password hash.
- Understand the basic workflow involved in password cracking.
- Document practical cybersecurity activities with screenshots.
- Analyze the security implications of weak or predictable passwords.
- Develop hands-on experience with cybersecurity assessment tools.
- Demonstrate practical ethical hacking and security-testing skills.

---

🧪 Laboratory Scope

The project consisted of two modules.

Module 1 — Password Cracking with John the Ripper

The first module focused on using John the Ripper (JTR) and its graphical interface, Johnny, to recover the password of a protected PDF.

The documented workflow included:

1. Installing/downloading John the Ripper.
2. Installing and configuring Johnny.
3. Locating the "john.exe" executable.
4. Obtaining the password hash from the protected PDF.
5. Saving the extracted hash into a text file.
6. Loading the hash file into Johnny.
7. Starting the password-cracking attack.
8. Waiting for the password-recovery process to complete.
9. Using the recovered password to open the protected PDF.

The project instructions identify John the Ripper as a password-cracking tool used by security professionals to test password strength and explain that Johnny provides a graphical interface for the tool.

---

Module 2 — Password Cracking with Networkwalks Tools

The second module provided an alternative web-based approach.

The Networkwalks Hash Calculator was used to extract the hash associated with the protected PDF, after which the extracted hash was submitted to the Networkwalks Password Cracker.

The workflow included:

1. Obtaining the protected PDF.
2. Opening the Networkwalks Hash Calculator.
3. Uploading the protected PDF.
4. Extracting the PDF hash.
5. Copying the complete hash.
6. Opening the Networkwalks Password Cracker.
7. Submitting the extracted hash.
8. Starting the password-recovery process.
9. Recording the recovered password.
10. Testing the recovered password by opening the protected PDF.

The lab documentation explains that the extracted PDF hash begins with "$pdf$" and that the complete hash must be copied before submitting it to the password-cracking tool.

---

🛠️ Tools Used

John the Ripper

John the Ripper is a password-security auditing and password-recovery tool capable of working with different types of password hashes.

In this project, it was used to demonstrate how a password-protected PDF can be assessed after its hash has been extracted.

Johnny

Johnny is the graphical user interface associated with John the Ripper.

Instead of relying entirely on command-line interaction, Johnny provides a graphical environment through which the password-recovery process can be configured and monitored.

The project instructions specifically use Johnny to open the extracted hash file and start a new attack.

Networkwalks Hash Calculator

The Networkwalks Hash Calculator was used to process the protected PDF and obtain the corresponding password hash.

The resulting hash was then used as input for the password-recovery stage.

Networkwalks Password Cracker

The Networkwalks Password Cracker was used to attempt password recovery from the extracted hash.

The lab documentation states that the tool tries different passwords until it finds a matching value.

Windows Laboratory Environment

The practical exercise was designed to be performed on a Windows computer. The project documentation also notes that the Networkwalks tools can be accessed through a web browser and that the JTR exercise can alternatively be performed on Kali Linux.

---

🧠 Key Concepts

Passwords

A password is an authentication secret used to control access to an account, application, file, or system.

Password security depends heavily on characteristics such as:

- Length
- Complexity
- Unpredictability
- Uniqueness
- Resistance to guessing
- Resistance to automated attacks

Weak and predictable passwords can significantly reduce the security of protected resources.

---

Hashing

Hashing converts input data into a corresponding hash value.

In password-security contexts, hashes can be used to represent passwords without storing the original password in plain text.

In this project, the protected PDF was processed to obtain the hash required for the password-recovery exercise.

The lab documentation describes hashing as a one-way process that transforms plaintext into a message digest.

---

Encryption vs Hashing

Encryption and hashing should not be treated as the same process.

Encryption is designed so that protected information can be recovered using the appropriate key.

Hashing, on the other hand, is designed as a one-way transformation.

This distinction is important when studying password security because the password-cracking process in this lab works with the extracted hash rather than directly reading the original password.

---

🔬 Methodology

The project followed a practical, evidence-based methodology.

Phase 1 — Preparation

The required software, web tools, protected PDF, and laboratory environment were prepared.

Screenshots were captured during important stages to provide evidence of the procedures performed.

Phase 2 — Hash Extraction

The password-protected PDF was processed to obtain the corresponding password hash.

For the JTR workflow, the extracted hash was saved into a text file before being loaded into Johnny.

For the Networkwalks workflow, the hash was obtained through the Networkwalks Hash Calculator.

Phase 3 — Password Recovery

The extracted hash was supplied to the appropriate password-recovery tool.

John the Ripper/Johnny was used for the first approach, while the Networkwalks Password Cracker was used for the second approach.

Phase 4 — Verification

After the password was recovered, it was entered into the protected PDF.

Successful opening of the PDF provided practical confirmation that the recovered password was correct.

The project documentation describes this verification step for both approaches.

Phase 5 — Documentation

Screenshots were collected and organized as evidence.

The screenshots demonstrate the progression from preparation and hash extraction through password recovery and verification.

---

📂 Module 1 — John the Ripper

Objective

The objective of Module 1 was to use John the Ripper and Johnny to recover the password protecting the supplied PDF.

Procedure

Step 1 — John the Ripper Installation

John the Ripper was obtained and prepared for use.

The official John the Ripper website is identified in the project instructions as one of the download sources.

Step 2 — Johnny Configuration

Johnny was opened and configured to use the John executable.

The required "john.exe" executable is located within the appropriate "run" directory according to the project instructions.

Step 3 — Obtain the PDF Hash

The password-protected PDF was processed using the specified hash-extraction method.

The resulting hash was copied for use during the password-recovery stage.

Step 4 — Create the Hash File

A text file named:

"hash1.txt"

was created.

The extracted hash was pasted into the file and saved for use with Johnny.

Step 5 — Load the Hash

The "hash1.txt" file was opened through Johnny using the password-file option.

Step 6 — Start the Attack

A new password-recovery attack was started.

The tool then attempted to identify a password corresponding to the supplied hash.

Step 7 — Password Verification

After the password was recovered, it was entered into the protected PDF.

The PDF successfully opened, demonstrating that the recovered password matched the password protecting the document.

---

📂 Module 2 — Networkwalks Tools

Objective

The objective of Module 2 was to perform the same general password-recovery task using Networkwalks web-based tools.

Procedure

Step 1 — Obtain the Protected PDF

The supplied encrypted PDF was obtained and prepared for testing.

Step 2 — Open Hash Calculator

The Networkwalks Hash Calculator was opened through a web browser.

Step 3 — Upload the Protected PDF

The protected PDF was uploaded to the Hash Calculator.

The tool processed the file and produced a PDF password hash.

Step 4 — Copy the Hash

The complete hash was copied.

Care was taken to preserve the full hash value because an incomplete hash would not provide the correct input for the next stage.

Step 5 — Open Password Cracker

The Networkwalks Password Cracker was opened.

Step 6 — Submit the Hash

The extracted hash was entered into the Password Cracker.

The password-recovery process was then started.

Step 7 — Observe the Result

The password-recovery process was allowed to complete.

The recovered password was displayed by the tool.

Step 8 — Verify the Password

The recovered password was entered into the original protected PDF.

The document opened successfully, confirming the result.

---

📸 Evidence and Screenshots

Screenshots were captured throughout the practical exercise to demonstrate the actual procedures performed.

The evidence is organized according to the two project modules.

Module 1 Evidence

Recommended evidence sequence:

1. John the Ripper installation/setup
2. Johnny interface
3. John executable configuration
4. PDF hash extraction
5. Hash file creation
6. Hash file loaded into Johnny
7. Password-recovery process
8. Recovered password/result
9. Successfully opened PDF

Module 2 Evidence

Recommended evidence sequence:

1. Networkwalks Hash Calculator
2. Protected PDF uploaded
3. Extracted PDF hash
4. Networkwalks Password Cracker
5. Hash submitted
6. Password-recovery result
7. Successfully opened PDF

Each screenshot should have a descriptive filename and caption rather than generic names such as "Screenshot1.png".

---

📊 Comparative Analysis

Area| John the Ripper / Johnny| Networkwalks Tools
Interface| Desktop/GUI| Web-based
Main purpose| Password recovery/testing| Password recovery/testing
Hash extraction| Separate extraction step| Hash Calculator
Password recovery| John the Ripper| Networkwalks Password Cracker
Configuration| More setup required| Minimal setup
Learning value| High| High
Practical cybersecurity value| Demonstrates professional password-auditing workflow| Demonstrates simplified browser-based workflow
Environment| Windows/Kali-compatible workflow| Browser-based

---

🔎 Findings

The practical exercise demonstrated several important observations.

Finding 1 — Password-protected files can be assessed through their hashes

The original password does not have to be directly visible for password-recovery testing to take place.

Once the appropriate hash is obtained, a password-cracking tool can attempt to identify a matching password.

Finding 2 — Weak passwords present a security risk

The successful recovery of the laboratory password demonstrates why predictable passwords should not be used to protect sensitive information.

The project documentation emphasizes that simple passwords can be recovered significantly more easily than stronger passwords.

Finding 3 — Hash protection does not automatically guarantee password strength

A hash may conceal the original password, but password security still depends on the strength of the underlying password and the security of the overall implementation.

Finding 4 — Multiple tools can accomplish similar security-testing objectives

The project demonstrated two different approaches to password recovery.

John the Ripper provided a more traditional password-auditing workflow, while the Networkwalks tools provided a simplified browser-based workflow.

Finding 5 — Evidence is important in cybersecurity

Capturing screenshots throughout the exercise provides a record of the actions performed and allows the practical results to be reviewed.

---

🛡️ Security Recommendations

Based on the lessons from this project, the following security controls are recommended.

1. Use strong passwords

Passwords should be sufficiently long and difficult to guess.

2. Avoid common passwords

Passwords such as:

- "123456"
- "password"
- Names
- Birth dates
- Simple patterns

should be avoided.

3. Use unique passwords

A password should not be reused across multiple systems or accounts.

4. Use a password manager

Password managers can help users create and maintain unique, complex passwords.

5. Enable Multi-Factor Authentication

Where available, MFA should be enabled to provide an additional authentication factor.

6. Protect sensitive files

Sensitive documents should use appropriate encryption and access controls.

7. Conduct authorized security testing

Password-cracking tools should only be used against systems, files, and accounts where the tester has explicit authorization.

---

⚖️ Ethical and Legal Considerations

Password-cracking tools are dual-use cybersecurity tools.

They can be valuable for:

- Security assessments
- Password auditing
- Cybersecurity education
- Penetration testing
- Incident response
- Defensive security research

However, attempting to recover passwords from systems or accounts without authorization can be illegal and unethical.

This project was conducted as a controlled educational laboratory exercise.

The purpose was to understand password security and demonstrate security-testing techniques rather than to gain unauthorized access to another person's information.

---

💡 Lessons Learned

This project provided practical experience in several areas of cybersecurity.

Technical Skills

- Password hash extraction
- Hash handling
- Password-recovery workflows
- John the Ripper
- Johnny GUI
- Web-based security tools
- File security
- Security testing
- Evidence collection

Analytical Skills

The project also required understanding the relationship between:

Protected File → Hash → Password-Recovery Tool → Recovered Password → Verification

Understanding this workflow provides a useful foundation for further cybersecurity studies.

Documentation Skills

The project also strengthened the ability to document technical procedures in a structured manner.

Rather than simply completing a practical task, each stage was recorded so that the process could be reviewed and reproduced within an authorized laboratory environment.

---

🚀 Future Improvements

Future versions of this project could expand the laboratory by examining:

- Different password strengths
- Different password attack strategies
- Password dictionaries
- Brute-force concepts
- Hybrid password attacks
- Password complexity analysis
- Hash types
- Password storage security
- Rate limiting
- Account lockout controls
- Multi-factor authentication
- Password-management policies

These areas would provide additional opportunities to study how organizations can defend against password-based attacks.

---

📁 Repository Structure

password-cracking-security-lab/
│
├── README.md
│
├── Module-1-John-the-Ripper/
│ ├── README.md
│ └── evidence/
│ ├── 01-john-installation.png
│ ├── 02-johnny-interface.png
│ ├── 03-john-configuration.png
│ ├── 04-pdf-hash.png
│ ├── 05-hash-file.png
│ ├── 06-hash-loaded.png
│ ├── 07-password-cracking.png
│ ├── 08-recovery-result.png
│ └── 09-pdf-verification.png
│
├── Module-2-Networkwalks/
│ ├── README.md
│ └── evidence/
│ ├── 01-hash-calculator.png
│ ├── 02-pdf-upload.png
│ ├── 03-extracted-hash.png
│ ├── 04-password-cracker.png
│ ├── 05-cracking-process.png
│ ├── 06-recovery-result.png
│ └── 07-pdf-verification.png
│
└── documentation/
    ├── Project-Module-1.pdf
    └── Project-Module-2.pdf

---

📌 Conclusion

This project provided a practical introduction to password security assessment and password-recovery techniques.

By completing the two modules, I gained hands-on experience with John the Ripper, Johnny, Networkwalks Hash Calculator, and Networkwalks Password Cracker.

The exercise demonstrated that password-protected files can be subjected to password-recovery attempts when the appropriate hash information is available. It also reinforced the importance of strong, unique passwords and appropriate security controls.

Most importantly, the project highlighted the value of performing cybersecurity testing within an authorized and controlled environment.

The knowledge gained from this laboratory exercise provides a foundation for further learning in ethical hacking, penetration testing, vulnerability assessment, cybersecurity operations, and defensive security.
