# SOAR-EDR-PROJECT

<h3>Introduction</h3>
This project provides a practical, hands-on walkthrough of deploying and integrating Security Orchestration, Automation, and Response (SOAR) within a Security Operations Center (SOC) environment. It leverages Tines as the SOAR platform and LimaCharlie as the Endpoint Detection and Response (EDR) solution to simulate real-world scenarios.

<h3>Key activities in the project include:</h3>

- Installing and configuring an EDR agent on an endpoint to explore its monitoring and response features.
- Crafting a custom detection rule to trigger alerts for password-recovery or credential-dumping tools.
- Automating incident notifications through both email and Slack channels.
- Executing automated EDR response actions, such as isolating compromised endpoints.

<h3>Tools and setup used: </h3>

- A virtualized environment (Windows 10 VM in this case).
- LimaCharlie for endpoint detection and response.
- Tines for workflow automation and orchestration.
- LaZagne for simulating credential-theft attempts.
- Email and Slack for alert and notification integrations.
