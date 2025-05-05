# Using-Wireshark---analyzing-web-browser-artifacts-email-header-analysis
# NAME:R.SABARINATH
# REGISTER NO:212223100048

# AIM:
To use Wireshark to analyze web browser activities and inspect email headers from captured network traffic.

# DESIGN STEPS:
Step 1:
Launch Wireshark and start capturing traffic on the appropriate network interface.

Step 2:
Use filters like http, dns, or tcp.port == 80 to monitor web browser artifacts such as visited URLs, cookies, and user-agent strings.

Step 3:
Apply filters like smtp, pop, or imap to locate and analyze email header details (e.g., sender, receiver, subject) from email communications.

# PROGRAM:
Wireshark Web and Email Traffic Filtering Steps

# A. Capturing Traffic in Wireshark
Open Wireshark and start capturing on the active interface (Wi- Fi/Ethernet).
![image](https://github.com/user-attachments/assets/ff840227-4fb1-4302-95b3-9d42dc0be528)

# Analyzing Web Browser Artifacts
Analyze Queries:
# FILTER HTTP:

![image](https://github.com/user-attachments/assets/da3033ec-490a-4464-8765-b0fadc31cecf)

# FILTER TCP:
![image](https://github.com/user-attachments/assets/a79eefcc-07b7-4cb2-9be6-2931d2ae6c56)

# APPLY RELAVANT FILTERS TCP.PORT=443
![Screenshot 2025-04-28 141058](https://github.com/user-attachments/assets/34a4cd95-76d4-4996-a955-f699871a6c09)
![Screenshot 2025-04-28 141805](https://github.com/user-attachments/assets/a9d08cdd-dc1b-458a-afda-b2fa6e931c91)
![Screenshot 2025-04-28 141832](https://github.com/user-attachments/assets/d38d82a1-b292-4390-b448-5a5f93304ad9)
# DNS :

![Screenshot 2025-04-28 141004](https://github.com/user-attachments/assets/a58fa0a4-3125-4ed2-a257-a84c122cc43a)

# Locate email data

Look for SMTP packets to see sender/receiver email addresses. Use "Follow TCP Stream" to view the full email headers and body if unencrypted.

# Extract Email Header Fields Analyze From, To, Subject, Date, Message-ID, and relay servers used in sending the email.
Perform activities like opening a website or sending an email through a client (e.g., Gmail via browser or Thunderbird).
![Screenshot 2025-04-28 141919](https://github.com/user-attachments/assets/836252c4-e1b0-44a8-9926-ac39e589e835)

Stop the capture once done.

