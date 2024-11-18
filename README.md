Overview- 
This repository contains the results of a vulnerability assessment I conducted on the PayMeFinTech website as part of a task for an internship application.

About Me- 
I am a student with a keen interest in cybersecurity. While I lack professional experience and access to advanced tools, I used freely available resources and techniques to perform this assessment. My knowledge is self-taught, and I attempted to apply what I learned to the best of my ability.


Tools Used- 
To identify vulnerabilities in the website, the following tools were employed:
Nikto: A web server scanner to detect outdated software, misconfigurations, and common vulnerabilities.
Wapiti: For identifying web application vulnerabilities like XSS, SQL injection, and file disclosure.
Skipfish: An active web application security reconnaissance tool.
Nslookup & Traceroute: To analyze DNS configurations and network paths.
Whois Lookup: To extract domain registration and hosting information.


Methodology- 
The assessment was conducted in the following steps:

1. Domain Information Gathering:
   - Used Whois to collect registrar details, DNS servers, and IP addresses.

2. Network Analysis:
   - Nslookup and Traceroute were utilized to evaluate DNS records and network routing.

3. Web Application Scanning:
   - Nikto, Wapiti, and Skipfish scans were conducted without authentication to discover potential vulnerabilities in the public-facing web application.


Findings- 
Below are the potential vulnerabilities identified during the assessment:

1. Outdated Software:
   - Nikto detected possible outdated versions of the web server software. This may leave the application susceptible to known exploits.

2. SSL/TLS Issues:
   - Skipfish identified weak SSL/TLS ciphers in use, potentially allowing attackers to intercept traffic.

3. Web Application Vulnerabilities:
   Wapiti scans highlighted:
     - XSS Risks: Input fields lacking proper sanitization.
     - Potential SQL Injection Points: Certain endpoints appear vulnerable due to improper input validation.


Recommendations- 
1. Update Software:
   - Ensure the web server and associated software are updated to their latest versions.

3. Enhance SSL/TLS Security:
   - Disable weak ciphers and implement a strong HTTPS configuration.

4. Mitigate Web Vulnerabilities:
   - Implement input sanitization and parameterized queries to prevent XSS and SQL injection.
   - Regularly test web applications using dynamic and static code analysis tools.



Conclusion- 
This project was a learning experience for me, the detailed findings and recommended mitigations should serve as a roadmap to strengthen the security posture of the PayMeFinTech website as per my understanding.

