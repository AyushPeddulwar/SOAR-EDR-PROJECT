# Installation & Configuration

---

### SETUP MESSAGING SYSTEM (Slack & Email) AND SOAR (Tines)

- **Setup Slack**

Set up a Slack account and create a channel for alerts. If you already have an account, just create a new channel for alerting.

![image.png](media/Installation%20&%20Configuration/image1.png)

### CREATE AUTOMATED WORKFLOW FROM EDR TO MESSAGING APPS VIA SOAR

**1. Connect LimaCharlie to Tines:** 
- Drag and drop Webhook from the left panel.
- Click the Webhook and fill in Name and Description fields.
- Copy the provided Webhook URL.
- In LimaCharlie, open your Organization → Outputs tab.
- Click Add Output.

![image.png](media/Installation%20&%20Configuration/image2.png)

- Confirm reciprocity on Tines: Click on the Webhook input. Click Events

![image.png](media/Installation%20&%20Configuration/3.png)

**2. Connect Slack & Email**

![image.png](media/Installation%20&%20Configuration/image3.png)

### Building SOAR Workflow

**1. LimaCharlie Alert Forwarding to Messaging Apps (Slack & Email):**

- Slack and Email input, we will change the message to include important information concerning the alert. The message should contain the following information:

<img src="media/Installation%20&%20Configuration/image4.png" width="400" height="450">

**2. Analyst Prompting:**

- Create a User Prompt.






