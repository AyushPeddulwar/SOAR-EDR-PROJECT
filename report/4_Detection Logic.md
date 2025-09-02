# ☁️ **Detection & Response Rule**

---
1. 
- Click on your Organization, and on the left, navigate to **Automation** > **D&R Rules** > **Add Rule**.
- Name the rule as desired.  
- Under **Detect**, enter the following configuration:

   ```yaml
   events:
     - NEW_PROCESS
     - EXISTING_PROCESS
   op: and
   rules:
     - op: is windows
     - op: or
       rules:
       - case sensitive: false
         op: ends with
         path: event/FILE_PATH
         value: LaZagne.exe
       - case sensitive: false
         op: contains
         path: event/COMMAND_LINE
         value: LaZagne
       - case sensitive: false
         op: is
         path: event/HASH
         value: 'PASTE-YOUR-HASH' 
   ```

2. **Define the Response Action**  
   - In the **Respond** field, enter the following:  

   ```yaml
   - action: report
     metadata:
       author: YOUR NAME
       description: TEST - Detects LaZagne Usage
       falsepositives:
         - ToTheMoon
       level: high
       tags:
         - attack.credential_access
     name: YOUR NAME - HackTool - LaZagne
   ```

![image.png](media/Detection%20Logic/image5.png)

3. **Create the Rule**  
   - Click the **Create** button to finalize the D&R rule.

4. **Verify Rule Execution**

![image.png](media/Detection%20Logic/1.png)