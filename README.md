# 📸 IoT Security Lab — Internet-Exposed Camera Exploitation  
> “The ‘S’ in IoT stands for *Security* — oh wait...there is no S”  
This lab explores the dangers of misconfigured IoT devices, focusing on Dahua IP cameras accessible over the internet. It combines Shodan-based reconnaissance with OSINT techniques to identify, fingerprint, and understand the real-world risks of exposed surveillance systems.

## 🎯 Objectives  
- Use Shodan to find internet-exposed Dahua cameras  
- Analyze open ports, banners, and default credentials  
- Capture screenshots of live camera feeds (where accessible)  
- Understand privacy implications and insecure default setups

## 🧰 Tools & Services  
- 🛰️ [Shodan.io](https://www.shodan.io)  
- 🧠 OSINT (IP Whois, GeoIP lookups)  
- 🌍 Web browser (for live interfaces)  
- 📁 Geo-coordinates for CIDR filtering

## 📌 Execution Workflow  
1. 🔍 **Shodan Dorks Used:**  
   ```sh
   title:"Dahua" country:"PK"  
   http.html:"DVRDVS-Webs"  
   port:37777  
   ```
2. 🌐 **Filtered Targets by Location:**  
   Applied custom coordinates & CIDRs to narrow down targets within Lahore, Pakistan  
3. 🔐 **Credentials Tested:**  
   Checked common default pairs like `admin:admin` and `admin:123456`  
   > 🚨 More than 70% of devices were still running default creds!  
4. 🖼️ **Snapshots Captured:**  
   Interfaces, settings pages, and even live camera feeds were saved (see screenshots)

## 📂 Lab Files  
- `IoT Security Lab.docx` – Complete documentation  
- `/screenshots/` – Real-world captures of exposed camera dashboards  
- Queries, filters, and banner data included

## ⚠️ Legal & Ethical Note  
All scans and analyses were done for educational purposes only. No exploitation, disruption, or unauthorized access was performed. Every step adhered to ethical hacking standards.

## 👨‍💻 Author  
**Sameer Malik** – Cybersecurity enthusiast passionate about Red Teaming & IoT Security  
GitHub: [mSameerMalik](https://github.com/mSameerMalik)  
LinkedIn: [linkedin.com/in/muhammad-sameer-malik-18b52634b](https://www.linkedin.com/in/muhammad-sameer-malik-18b52634b/)

## 🏷️ Tags  
#IoTSecurity #Shodan #OSINT #Dahua #CameraHacking #CyberAwareness #RedTeam #Infosec #EthicalHacking #mSameerMalik
