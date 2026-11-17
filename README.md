Week 3 – Password Cracking (JTR & Networkwalks Tools)

Cybersecurity & Ethical Hacking project work — Networkwalks Academy, Batch B084.

This repo documents two methods used to recover the password of an encrypted PDF file (My Locked PDF1.pdf), as part of Week 3's essential project modules.

Modules
PM1 – Password Cracking with JTR

Tools: John the Ripper (CLI) + Johnny (GUI front-end), on Windows.

Steps performed:

Extracted the PDF's crackable hash using pdf2john (via the Online Hash Crack PDF Hash Extractor) and saved it as a hash file.
Loaded the hash file into Johnny.
Confirmed the John the Ripper executable path in Johnny's Settings.
Ran a dictionary attack against the hash.
Recovered the password and used it to unlock the PDF.

Screenshots: PM1 - JTR (JohnJohny)/

PM2 – Password Cracking with Networkwalks Tools

Tools: Networkwalks Hash Calculator + Networkwalks Password Cracker (browser-based, no installation required).

Steps performed:

Uploaded the PDF to the Hash Calculator to extract its $pdf$... hash.
Pasted the hash into the Password Cracker.
Ran the built-in dictionary attack.
Recovered the password and used it to unlock the PDF.

Screenshots: PM2 - Networkwalks tools/

Result

Both methods independently recovered the same password, confirming the result. This highlights how quickly a weak, common password can be cracked with freely available tools — regardless of whether the attack is run from the command line or a simple browser tool.

Key takeaway

Password strength matters more than the tool used to attack it. A short, dictionary-word password falls to both a local CLI tool and a public web tool in seconds. Strong, unique passwords (length, mixed character types, not based on dictionary words) remain the most effective defence against this class of attack.

Disclaimer

This work was carried out in a controlled training environment on a file provided for the exercise, for educational purposes only, as part of the Networkwalks Cybersecurity & Ethical Hacking course.

Author: Gabriel Chilufya
Course: Networkwalks Cybersecurity & Ethical Hacking, Batch B084
