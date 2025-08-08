# NetOS-Detect: Automated OS Detector:

NetOS-Detect is a powerful and modular tool for network administrators and security
professionals to automatically discover and identify the operating systems of devices
on a network. It combines passive analysis with active scanning techniques to provide
an accurate inventory of network assets.

🚀 Features

● Host Discovery: Automatically discovers live hosts on a target network using ARP
and ICMP scans.

● Passive Fingerprinting: Identies operating systems stealthily by analyzing
existing network trac (e.g., TTL, TCP Window Size, Banners).

● Active Scanning: Performs sophisticated active scans using craed packets to
accurately determine the OS of target hosts.

● Reporting: Generates reports on network composition and discovered devices.

● Modular Architecture: Easy to extend with new detection techniques and
features.

⚙️ Installation and Setup

Follow these steps to get the project running on your local machine.

Prerequisites:

● Python 3.8+

● pip (Python package installer)

● libpcap or Npcap (for packet capturing with Scapy).

○ Linux (Debian/Ubuntu): sudo apt-get install libpcap-dev

○ Windows: Install Npcap during the Scapy installation process.

1. Clone the repository:

   
   git clone https://github.com/Richie13root/NetOS-Detect.git

   cd NetOS-Detect

2. Create a virtual environment (recommended):
   
   python -m venv venv
   
   source venv/bin/activate # On Windows use `venv\Scripts\activate`

3. Install dependencies:
   
   pip install -r requirements.txt

 ️ Usage:
 
  The core detection logic can be run from the command line. You must run the script
  with administrator/root privileges to allow for raw socket operations.

  On Linux/macOS

  sudo python detector.py --target 192.168.1.1

  On Windows (in an Administrator terminal)

  python detector.py --target 192.168.1.1  

  ⚠️ Ethical and Legal Disclaimer
  
This tool is intended for educational purposes and for authorized use only.
Unauthorized scanning of networks is illegal and unethical. The user is responsible for
their actions and must have explicit, wrien permission from the network owner
before using this tool. The developers of this project are not responsible for any
misuse or damage caused by this program. Always respect privacy and the law.

 📄 License
 
This project is distributed under the MIT License. See the LICENSE for more
information.



