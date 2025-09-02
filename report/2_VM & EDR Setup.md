# VM & EDR Setup

This step involves installing and configuring Lima Charlie’s Endpoint Detection and Response (EDR) on a Windows 10 machine.
You can set up a Windows 10 VM locally or via a cloud provider, ensuring it has internet access.
For this project, Lima Charlie was the chosen EDR solution.

| Component | Role | Location | OS
| --- | --- | --- | ---- |
| `Win10 Victim` | Log Source | VMware(Local) | Win 10 x64 |
| `LimaCharlie` | EDR Platform | - | - |
| `Tines` | SOAR Platform | - | - |
| `Slack` | Real time alert | - | - |

---

### ⚙️ Deployment Breakdown

### 💻 **Windows 10 VM**  

![image.png](media/VM%20&%20EDR%20Setup/image1.png)

- Acts as the victim machine
- Sends logs to the LimaCharlie over the internet
- Tools:<br>
       - EDR Agent Installation (configure to push endpoint data to our LimaCharlie Organization)<br>
       - "LaZagne" (credential stealer malware)

![image.png](media/VM%20&%20EDR%20Setup/image2.png)

### ☁️ **LiamCharlie**

![image.png](media/VM%20&%20EDR%20Setup/image3.png)
<br> <br>
![image.png](media/VM%20&%20EDR%20Setup/image4.png)

- Collects and analyzes logs from Windows client



