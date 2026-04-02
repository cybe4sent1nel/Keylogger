# Advanced Python Keylogger

**Author:** cybe4sent1nel (Fahad Khan)

## ⚠️ Legal Disclaimer & Ethical Guidelines
**STRICTLY FOR EDUCATIONAL AND ETHICAL HACKING PURPOSES ONLY.**

This tool is a legitimate penetration testing utility designed to demonstrate system vulnerabilities and the mechanics of local data logging, functioning conceptually similar to auditing tools like Hashcat or airgeddon. It is intended solely for use in controlled, explicitly authorized environments, such as academic internship projects or dedicated security labs. 

Any misuse of this software to intercept data, monitor individuals without their explicit consent, or gain unauthorized access to systems is illegal and strictly prohibited. The author assumes no liability and is not responsible for any misuse, damage, or legal consequences caused by this program. By utilizing this tool, you agree to abide by these strict ethical guidelines.

## Features
* **Keystroke Monitoring:** Captures and logs all keyboard inputs dynamically.
* **Peripheral Tracking:** Logs mouse movements, clicks, and scroll events.
* **System Profiling:** Gathers host information including hostname, IP address, processor architecture, and OS details.
* **Audio Recording:** Captures environmental microphone input for specified intervals.
* **Visual Logging:** Captures and transmits screenshots of the current display.
* **Automated Exfiltration:** Dispatches compiled text logs, audio files, and images via SMTP (e.g., Mailtrap) at defined intervals.
* **Self-Destruct Sequence:** Features built-in process termination and file-deletion routines to clear traces post-execution on both Windows and Unix-like systems.

## Prerequisites & Installation

The script includes an automatic dependency installer, but you can also install the requirements manually using the provided `requirements.txt`.

```bash
pip install -r requirements.txt
Required Libraries:

pynput==1.7.3

pyscreenshot==0.5.1

sounddevice==0.4.3

Pillow==9.3.0

Configuration
Before deploying the tool in your authorized testing environment, configure your SMTP credentials and reporting intervals directly within keylogger.py:

Python
EMAIL_ADDRESS = "YOUR_USERNAME"
EMAIL_PASSWORD = "YOUR_PASSWORD"
SEND_REPORT_EVERY = 60 # Execution and report interval in seconds
Usage
Execute the script from the terminal or command prompt:

Bash
python keylogger.py
Note: Depending on your operating system's security policies, this script may require administrative or root privileges to successfully hook into global input events.

Support & Funding
If you found this tool helpful for your educational research or penetration testing studies, consider supporting its continued development:

PayPal: fahadkhanxyz8816@gmail.com
