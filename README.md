Web Application Penetration Testing and Incident Response using DVWA

Project Overview
This project demonstrates a web application penetration test performed on DVWA (Damn Vulnerable Web Application) hosted on a Metasploitable machine. The aim of the project is to identify common web vulnerabilities, exploit them in a controlled environment, and understand their impact on system security. In addition, an incident response simulation was carried out to detect and mitigate the attacks.

Objective
The main objective of this project is to analyze the security of a web application by identifying vulnerabilities such as SQL Injection, Cross-Site Scripting (XSS), and Command Injection. The project also focuses on understanding how these vulnerabilities can be exploited and how to defend against them.

Lab Environment
The project was conducted in a virtual lab setup. Kali Linux was used as the attacker machine, while Metasploitable was used as the target system hosting DVWA. Both systems were connected through a virtual network.

Tools Used
1. Kali Linux was used as the primary platform for performing attacks. DVWA was used as the vulnerable web application.
2. Metasploitable served as the target machine. 
3. Nmap was used for scanning and reconnaissance.
4. Gobuster for directory enumeration, and 
5. web browser for manual testing. 
6. Firewall rules were applied using iptables during the incident response phase.

Methodology
The project was carried out in multiple phases.
1. In the reconnaissance phase, Nmap was used to scan the target system and identify open ports and running services.
2. In the enumeration phase, Gobuster was used to discover hidden directories and locate the DVWA application.
3. In the exploitation phase, multiple vulnerabilities were tested and exploited:
4. SQL Injection was performed to bypass authentication and retrieve database records.
5. Cross-Site Scripting (XSS) was used to inject and execute JavaScript code in the browser.
6. Command Injection was performed to execute system-level commands on the target machine.

Findings
1. The testing revealed several vulnerabilities in the application.
2. SQL Injection was identified as a high severity vulnerability, allowing unauthorized access to database records.
3. Cross-Site Scripting was identified as a medium severity vulnerability, enabling execution of malicious scripts in the user's browser.
4. Command Injection was found to be a critical vulnerability, allowing execution of system commands.
5. Open ports and exposed services increased the overall attack surface of the system.

Mitigation Strategies
1. To prevent SQL Injection, prepared statements and proper input validation should be used.
2. To prevent XSS, user inputs should be validated and output should be properly escaped. Implementing Content Security Policy can also help.
3. To prevent Command Injection, direct execution of system commands should be avoided and secure APIs should be used.
4. In general, enabling firewalls, disabling unnecessary services, and performing regular security testing can improve system security.

Incident Response Simulation
1. An incident response simulation was performed to understand how attacks can be detected and mitigated.
2. Apache access logs were monitored using the tail command to detect suspicious requests containing malicious payloads.
3. Once the attack was identified, the attacker’s IP address was blocked using firewall rules through iptables.
4. This helped in preventing further malicious activity and demonstrated how quick response can reduce the impact of an attack.

Project Structure
The repository contains the project report, screenshots of each step, and supporting files related to the penetration testing process.

Conclusion
This project demonstrates how common web vulnerabilities can be exploited and highlights the importance of secure coding practices. It also shows how monitoring and incident response play a crucial role in protecting systems from cyber attacks.

Author
Divya Shukla  
