# 🔒 Linux CIS Benchmark Audit Tool  

This tool helps audit Linux systems based on **CIS (Center for Internet Security) benchmarks** to improve security. It performs various security checks and generates compliance reports.  

## 🚀 Features  
✅ CIS benchmark compliance checking  
✅ Generates audit reports in a structured format  
✅ Easy installation via `.deb` package  
✅ Lightweight shell script for quick execution  

## 📌 Installation  

### **1️⃣ Install Using .deb Package**  
You can install the tool using the provided Debian package:  
sudo apt install ./audit-tool.deb

If any dependency issue occurs, fix it using:
sudo apt --fix-broken install

### **2️⃣ Run Directly Using Shell Script
If you don’t want to install, you can run the audit script directly:
chmod +x cis_audit.sh
./cis_audit.sh


### **🛠️ Usage
### **1️⃣ Run a Full System Audit
./cis_audit.sh --full
This will perform a full security audit based on CIS guidelines.

### **2️⃣ Run a Specific Check
Example: Checking SSH security
./cis_audit.sh --check ssh

### **3️⃣ Generate an Audit Report
To save audit results to a log file:
./cis_audit.sh --report audit_report.log

### **📊 Output Format
The script generates reports in the following format:
[+] Checking SSH Configuration... PASSED  
[-] Checking Firewall Rules... FAILED  
[!] Checking User Permissions... WARNING  

### **📜 License
This project is licensed under the MIT License - see the LICENSE file for details.
