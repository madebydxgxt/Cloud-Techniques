# servicenow-ticket-provisioning-powershell

A hands-on lab demonstrating how to provision (create) ServiceNow incident tickets by sending a REST API payload from a PowerShell script.

## Watch me build this lab
https://www.loom.com/share/3279ef8336d54e54b0492462505d576d

**What this video shows:** Running a PowerShell script that posts an incident payload to a ServiceNow developer instance and then verifying the created ticket inside the Incident list.

---

## Objective
Automate the creation of ServiceNow incident tickets by pushing data to a ServiceNow instance using a PowerShell script.

---

## Skills Practiced
- PowerShell scripting for automation
- Working with a ServiceNow Developer Instance
- Calling REST APIs from PowerShell (Invoke-RestMethod)
- Basic authentication / credential handling (high-level)
- Building and sending a request payload (example: JSON body)
- Interpreting API responses (success flags + returned identifiers)
- Verifying records in ServiceNow (Incident table search)
- Basic troubleshooting when records don’t immediately appear

---

## Tools Used
- ServiceNow Developer Instance
- ServiceNow Incident table/module
- Windows PowerShell (PowerShell terminal)
- ServiceNow REST/Table API (example: Incident endpoint)
- (Optional) Text editor or IDE for script review (example: VS Code)

---

## Steps Performed
## Provisioning Tickets in ServiceNow Using PowerShell

### Objective

This SOP outlines the steps to provision tickets into ServiceNow using a PowerShell script for automation, particularly for bulk updates.

### Key Steps

**1. Prepare Your Environment** [0:02](https://loom.com/share/a401750e284d407690e7d73426b871dc?t=2)

![image alt](

- Open your PowerShell terminal.
- Ensure you have access to your ServiceNow developer instance.

**2. Copy the PowerShell Script** [0:26](https://loom.com/share/a401750e284d407690e7d73426b871dc?t=26)



- Copy the provided PowerShell script.
- Make sure to replace the placeholder values with your actual developer instance, username, and password.

**3. Paste the Script in PowerShell** [1:04](https://loom.com/share/a401750e284d407690e7d73426b871dc?t=64)



- Paste the modified script into your PowerShell terminal.

**4. Execute the Script** [1:12](https://loom.com/share/a401750e284d407690e7d73426b871dc?t=72)



- Run the script to push the data to ServiceNow.

**5. Retrieve Task Effective Number** [1:23](https://loom.com/share/a401750e284d407690e7d73426b871dc?t=83)



- After execution, note the task effective number from the output.

**6. Search for the Incident in ServiceNow** [2:00](https://loom.com/share/a401750e284d407690e7d73426b871dc?t=120)



- Log into your ServiceNow instance.
- Navigate to the incidents section.
- Use the task effective number to search for the newly created incident.

**7. Verify the Incident** [2:26](https://loom.com/share/a401750e284d407690e7d73426b871dc?t=146)



- Confirm that the incident appears in the search results.

### Cautionary Notes

- Ensure that you have the necessary permissions to access and modify ServiceNow data.
- Double-check your username and password to avoid authentication errors.

### Tips for Efficiency

- Use a text editor to modify the PowerShell script before pasting it into the terminal to avoid syntax errors.
- Keep a record of the task effective numbers for future reference.

---

## Outcome
Successfully created a ServiceNow incident via a PowerShell REST call and confirmed the new ticket appeared in the ServiceNow Incident list.
