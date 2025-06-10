# burp-suite-web-vuln-lab
Educational Burp Suite web vulnerability testing lab with intercept, scan, and exploit examples using DVWA/Juice Shop. Includes IP/port config guidance for learners.
# 🕷️ Web Application Tester using Burp Suite

> 🔒 **Educational and Ethical Use Only**  
This project is a demonstration of how to use [Burp Suite](https://portswigger.net/burp) to test web application security vulnerabilities in a controlled environment or lab setup. Do not test websites or systems without **explicit permission**.

---

## 🎯 Project Goal

This repo shows how to:
            - Intercept and modify HTTP/S requests using Burp Suite
            - Scan for common web vulnerabilities
            - Exploit test flaws (e.g., XSS, SQLi, IDOR)
            - Automate scanning with Burp Suite’s tools

---

## 🛠️ Tools Used

| Tool           | Purpose                                      |
|----------------|----------------------------------------------|
| Burp Suite     | Intercept & analyze web traffic              |
| OWASP Juice Shop / DVWA | Vulnerable test targets              |
| Firefox + FoxyProxy | Burp integration                        |
| SQLMap / XSS Hunter (optional) | Manual exploitation follow-up |

---

## 🧪 Features Demonstrated

### 🔍 Intercepting Requests

```plaintext
- Change form fields before submission
- Modify cookies or tokens
- Observe headers & hidden parameters

🧬 Vulnerability Scanning
            -Active/Passive scans
            -Crawler to discover hidden content
            -Custom scan policies (SQLi, XSS, Open Redirects, etc.)

💣 Manual Testing with Repeater & Intruder
            -Fuzz login forms with wordlists
            -Replay modified GET/POST requests
            -Enumerate IDOR endpoints

🚀 Quick Start
1. Set Up Burp Suite Community Edition

sudo snap install burpsuite
2. Launch a Vulnerable Web App (DVWA or Juice Shop)

docker run -d -p 3000:3000 bkimminich/juice-shop

3. Set Up Browser Proxy (e.g., Firefox to 127.0.0.1:8080)

4. Start Intercepting
Visit web app in browser

Capture requests in Burp > Proxy > HTTP history


🧠 Key Use Cases
Test login forms for brute force / credential stuffing

Analyze session handling and token rotation

Detect reflected/stored XSS

Probe for SQLi and IDOR vulnerabilities

📁 Folder Structure

.
├── test_reports/
│   └── juice-shop_scan.html
├── payloads/
│   └── fuzz_usernames.txt
├── screenshots/
├── README.md
📚 Recommended Learning Targets
Concept	Resource
OWASP Top 10	https://owasp.org/www-project-top-ten/
Burp Suite Guide	https://portswigger.net/burp/documentation
DVWA	http://www.dvwa.co.uk/

 Legal Usage
Only test:

Applications you own

Authorized lab environments (e.g., Juice Shop, DVWA, WebGoat)

With clear permission from system owners

🧠 Learning Outcomes
Understand how HTTP requests can be manipulated

Learn how common vulnerabilities appear in real-world apps

Use Burp Suite for both automated and manual testing

Write and analyze vulnerability reports


🤝 Contributing
Feel free to:

Add new testing scenarios (e.g., SSRF, command injection)

Include real-world writeups (responsibly disclosed)

Submit better fuzz payloads

markdown


---

### 🔖 Suggested Repo Name:
- `burp-suite-web-tester`
- `web-vulnerability-lab-burp`
- `burp-intercept-and-scan`

Would you like me to generate:
- Sample reports (`juice-shop_scan.html`)?
- Custom payload lists (for fuzzing)?
- A full lab setup guide with Docker?


To Configure Ip, Port and to import CA Certificate of burp suite refer to the link below given link:
https://github.com/obitonohara/Burp-Suite-IP-and-Certificate
