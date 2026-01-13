# Phishing-Project-

Project Description-
This project demonstrates the working principle of phishing attacks using the open-source framework Zphisher, executed in a controlled Linux environment.
The objective is to understand how phishing toolkits operate, how fake login pages are generated, and how attackers attempt to collect user credentials — strictly for educational and awareness purposes.

System Environment Used-
Host OS: Windows
Linux Environment: Ubuntu via Windows Subsystem for Linux (WSL)
Tool Used: Zphisher (open-source phishing simulation framework)
WSL was chosen to avoid using a full virtual machine while still maintaining a Linux-based testing environment.

Project Workflow (Conceptual)-

1️. Linux Environment Initialization
The project begins by launching Ubuntu using WSL from the Windows command line.
This provides a Linux terminal where security tools can be executed safely in isolation from the host system.

2️. Repository Acquisition
The Zphisher source code is obtained from its official GitHub repository and stored locally within the Ubuntu file system.
This repository contains:
Shell scripts
Web templates
Local hosting configurations

3️. Toolkit Execution
After navigating into the project directory, the main Zphisher script is executed.
This launches a command-line interface (CLI) that allows users to select different simulated phishing scenarios.
At this stage:
Required dependencies are verified
The phishing framework initializes its internal services

4️. Selection of Phishing Template
For demonstration purposes, an Instagram login page template is selected.
The tool then generates a replica of the original login interface, visually similar to the real website.
This step helps demonstrate:
How attackers mimic trusted platforms
Why users may fail to distinguish fake pages from legitimate ones

5️. Local Hosting and Port Forwarding
The generated phishing page is hosted locally.
To make the page reachable for demonstration, a port forwarding service (Cloudflared) is selected.
Cloudflared:
Creates a temporary public tunnel
Automatically assigns a port
Maps the local server to a public-facing URL
No custom port configuration is used in this project.

6️. Demonstration of Data Capture Mechanism
When a user enters login credentials into the simulated page:
The data is captured by the local server
Information is logged within the tool’s environment
This demonstrates:
How phishing tools collect sensitive data
Why phishing is dangerous
How attackers exploit human trust rather than technical vulnerabilities

All credentials used during testing were dummy/test data, and no real accounts were targeted.

Key Learning Outcomes-
This project helps in understanding:
The internal workflow of phishing frameworks
The role of port forwarding in exposing local services
How realistic phishing pages are generated
Why phishing attacks are effective
The importance of cybersecurity awareness and user education

Ethical Considerations-
This project was performed only in a controlled environment
No real individuals were targeted
No real credentials were collected
The project complies with ethical hacking principles
Misuse of such tools outside authorized testing environments is illegal.

Academic Relevance-
This project is relevant to:
Cybersecurity fundamentals
Ethical hacking
Network security
Social engineering analysis
Secure system design

Conclusion-
By simulating a phishing attack workflow, this project highlights how easily users can be deceived and emphasizes the need for:
User awareness training
Strong authentication mechanisms
Phishing detection systems
The focus of this project is learning and prevention, not exploitation.
