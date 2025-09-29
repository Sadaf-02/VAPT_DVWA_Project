# VAPT_DVWA_Project
🔒 Vulnerability Assessment and Penetration Testing (VAPT) on DVWA
📌 Project Overview

This project focuses on performing a Vulnerability Assessment and Penetration Testing (VAPT) on the Damn Vulnerable Web Application (DVWA).
DVWA is a deliberately insecure PHP/MySQL web application that is widely used to practice and demonstrate common web vulnerabilities.

The objective of this project was to:

Understand different types of vulnerabilities in web applications.

Perform attacks on DVWA in different security levels.

Document the findings with methodology, exploitation process, and prevention measures.

Gain hands-on skills in penetration testing using tools like Burp Suite, SQLMap, and Kali Linux utilities.

🛠 Tools & Technologies Used

Operating System: Kali Linux

Target Application: DVWA (Damn Vulnerable Web Application)

Web Server: Apache (via XAMPP)

Database: MySQL

Testing Tools:

Burp Suite

SQLMap

Browser DevTools

Hydra

Linux Command-Line Utilities

🔍 Methodology Followed

The standard VAPT Methodology was followed in this project:

Information Gathering – Collected details about DVWA environment.

Scanning & Enumeration – Checked open ports, services, and potential entry points.

Vulnerability Assessment – Identified vulnerabilities using both manual and automated techniques.

Exploitation – Performed attacks to exploit discovered vulnerabilities.

Reporting & Documentation – Documented methodology, exploitation process, and mitigations.

⚡ Vulnerabilities Tested in DVWA

The following vulnerabilities were assessed and exploited:

Brute Force Attack – Attempted login bypass using Burp Suite Intruder & Hydra.

Command Injection – Executed system-level commands through insecure inputs.

Cross-Site Request Forgery (CSRF) – Forced a logged-in user to perform unwanted actions.

Cross-Site Scripting (XSS)

Reflected XSS

Stored XSS

SQL Injection (SQLi) – Extracted database information using SQL queries and SQLMap.

File Inclusion – Explored Local File Inclusion (LFI) and Remote File Inclusion (RFI).

Insecure Captcha & Weak Security Configurations – Tested captcha bypass and weak settings.

Cryptography Weakness – Explored password hashing mechanisms.

📸 Screenshots & Demonstrations

Screenshots of each attack and proof of concept are included in the docs/screenshots/ folder.
Each screenshot demonstrates:

Attack vector

Payload used

Successful exploitation result

📝 Findings & Recommendations

Vulnerability	Impact	Exploitation	Mitigation
SQL Injection	High	Extracted DB tables	Use Prepared Statements, Parameterized Queries
XSS (Stored & Reflected)	High	Session Hijacking, Cookie Theft	Input Validation, Output Encoding
Command Injection	Critical	Executed arbitrary system commands	Restrict system calls, Input sanitization
CSRF	Medium	Unauthorized state changes	Implement CSRF Tokens
Brute Force	Medium	Password guessing	Implement Account Lockout, Strong Password Policy
File Inclusion	High	Arbitrary File Access	Restrict file paths, Use allowlist
📖 Conclusion

This project provided a practical understanding of how attackers exploit web applications and the importance of secure coding practices.
By performing VAPT on DVWA, I learned how to:

Identify common web vulnerabilities.

Exploit them using different tools and payloads.

Recommend effective countermeasures to strengthen security.

The knowledge gained from this project builds a strong foundation for pursuing advanced penetration testing and cybersecurity research.

📚 References

DVWA Official GitHub

OWASP Top 10 – OWASP Website

Kali Linux Tool Documentation

👨‍💻 Author

Sadaf Rasool

🎓 B.Tech in Computer Science & Engineering (3rd Year)

🔐 Interested in Cybersecurity and Penetration Testing

🌐 GitHub: your-username
