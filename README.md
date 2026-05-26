# Creating-and-Analyzing-Packets-Lab
---
# Objective 
 - Create a Packet Capture using Wireshark
 - Create a Packet Capture within the Palo Alto Networks Firewall 
 - Analyze PCAP Files with Wireshark
---

# Tools Used
- Wireshark
- NETLAB+
- Palo Alto Networks PAN-OS
---

# Load Lab Configuration
 ---
 
 ### In this section, I will load the Firewall configuration file. Click on Client tab to access the Client PC
<img width="866" height="69" alt="Screenshot 2026-05-26 093100" src="https://github.com/user-attachments/assets/5d8190a8-03b5-4478-9860-1eddfcfda663" />

### Login to the Client PC. Once you are signed in double click the google chrome icon on the desktop
<img width="81" height="136" alt="Step 2" src="https://github.com/user-attachments/assets/6b8fc0a2-2688-41e9-869d-28d2a3d4fba9" />

### Type in https://192.168.1.254 in the google chrome search bar and then press enter
<img width="417" height="86" alt="image" src="https://github.com/user-attachments/assets/964b014c-fce9-4135-9fcd-de9df7ab7490" />

###  A message will appear and say “Your connection is not private” message. Click on the ADVANCED link
<img width="816" height="432" alt="Step 5" src="https://github.com/user-attachments/assets/9aafd898-0106-4986-852d-61f043713c6b" />

### After Clicking on the ADVANCED link click on Proceed to 192.168.1.254 (unsafe)
<img width="829" height="577" alt="Step 6" src="https://github.com/user-attachments/assets/ed9661e4-ccff-40ae-a96d-2aaf06acfd56" />

### Login into Paloalto and click login
<img width="531" height="411" alt="Screenshot 2026-05-26 165535" src="https://github.com/user-attachments/assets/2381fcf2-e6ce-415b-9429-5af67c6c78a5" />

### In the web interface, navigate to Device > Setup > Operations and click on Load named configuration snapshot underneath the Configuration Management section.
<img width="825" height="388" alt="image" src="https://github.com/user-attachments/assets/7606fc3e-3c88-4f55-9c68-ce960aca7ac3" />

### In the Load Named Configuration window, select pan8-cg-lab-04 from the Name dropdown box and click OK then close it.
<img width="473" height="182" alt="Screenshot 2026-05-26 170427" src="https://github.com/user-attachments/assets/737a4341-a38f-4de4-9a33-d10fa9e385ab" />
<img width="480" height="174" alt="Screenshot 2026-05-26 170440" src="https://github.com/user-attachments/assets/802e612b-df3c-48a0-84c4-d33d3629febd" />

### Next you want to Click the Commit link located at the top-right of the web interface.
<img width="311" height="84" alt="Screenshot 2026-05-26 170844" src="https://github.com/user-attachments/assets/23083efe-2125-47f8-9831-093d473d4120" />

###  In the Commit window, click Commit to proceed with committing the changes. After doing this When the commit operation successfully completes, click Close to continue.
<img width="700" height="387" alt="Screenshot 2026-05-26 171147" src="https://github.com/user-attachments/assets/1da066e5-62e1-4ee2-8681-7ba9256a08a0" />
<img width="594" height="245" alt="Screenshot 2026-05-26 171202" src="https://github.com/user-attachments/assets/df134d46-d21b-4cbc-8d63-c039b248785c" />

### The commit process takes changes made to the Firewall and copies them to the running configuration, which will activate all configuration changes since the last commit.
---
# Creating a Wireshark Packet Capture

### Click on the Windows icon in the bottom-left corner then click on Wireshark
<img width="437" height="567" alt="Screenshot 2026-05-26 172521" src="https://github.com/user-attachments/assets/8e206d63-bebe-4338-8dc3-ef36a9ce8581" />

### Once Wireshark opens click on the internal interface from the list. Go to Capture> Start
<img width="664" height="312" alt="Screenshot 2026-05-26 172826" src="https://github.com/user-attachments/assets/ee3c727b-4233-4138-9871-cffcac248a88" />
<img width="450" height="354" alt="Screenshot 2026-05-26 172842" src="https://github.com/user-attachments/assets/ca56a9ea-5709-454e-9010-9af08fbb05a6" />

### Minimize Wirewark
<img width="190" height="116" alt="Screenshot 2026-05-26 173736" src="https://github.com/user-attachments/assets/f1473f98-919f-4926-bd0f-cc03ad7b0895" />

### Go to Google Chrome and create a new tab
<img width="534" height="73" alt="Screenshot 2026-05-26 173752" src="https://github.com/user-attachments/assets/691018cb-b42d-44bc-8a2b-6461d204a65b" />

### In the Search bar type http://www.panlabs.com and press Enter.
<img width="535" height="69" alt="Step 19" src="https://github.com/user-attachments/assets/c8d99e52-20a6-47b3-a63a-c9fca744c3ef" />

### After pressing enter Wait 5 to 10 seconds and reopen Wireshark and then click the Stop capturing packets button. 
<img width="1194" height="579" alt="Step 20" src="https://github.com/user-attachments/assets/86eeb688-43fc-4fa5-8edf-d8ce20c5e5c6" />

### To save the Wireshark packet capture, click on File > Save As
<img width="320" height="503" alt="Step 21" src="https://github.com/user-attachments/assets/5bba6e5c-49ce-4e0c-bf73-39b2a093f7a5" />

###  In the Save file as window, click on Desktop on the left. Then, type packetcapture in the File name field. Finally, click Save.
<img width="653" height="511" alt="Step 22" src="https://github.com/user-attachments/assets/dfdfa6ff-81fd-4162-8f23-bcc42f56015b" />

# Results of Lab 

### When I used Wireshark, I located the ARP request who has 192.168.1.254 which is one line 215 followed by the reply 192.186.1.1 which is on line 216. The DNS is at line 217 the that says standard query 0xa7e7 A clients1.google.com
<img width="1048" height="520" alt="Results of Lab" src="https://github.com/user-attachments/assets/0c556b5b-3161-4163-a358-a72dc78b7219" />














