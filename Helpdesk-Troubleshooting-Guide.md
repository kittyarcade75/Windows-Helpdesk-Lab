# Purpose 
This guide will document a repeatable process for diagnosing common Windows 11 support issues. It will focus on gatherin symptoms, performing safe checks, documenting findings, and escelating problems when necessary. 

# Lab Enviornment
**Operating System:** Windows 11 

**Tools:** Windows settings, Windows PowerShell, built-in Windows troubleshooting tools

**Environment:** personal practice lab 

# Standard Troubleshooting Process
1. Identify the user's reported problem.
2. Ask when the issue started and whether anything changed recently (ex: upates).
3. Record the exact error message, if any.
4. Check simple causes before attempting advanced fixes.
5. Perform one diagnostic step at a time.
6. Record the result of each step.
7. Apply an appropriate fix only when justified
8. Verify whether the problem is resolved.
9. Escalate unresolved issues with clear notes.

# Scenario One: No Internet Connection
**Reported symptoms:** a user reports that their Windows computer cannot access the internet 

<ins>Diagnostic Steps</ins>
1. Check whether Wi-Fi is enabled and the computer is connected to the expected network.
2. Run the command "ipconfig /all" in PowerShell to inspect network configuration.
3. Run the command "1.1.1.1" in PowerShell to test connectivity to an external IP address.
4. Run the command "nslookup (insert domain)" in PowerShell to test DNS resolution.
5. Compare the results to identify the likely area of failure.

<ins>Documentation</ins>
1. Checked Wi-Fi status: Windows showed Wi-Fi as connectedl
2. Checked IP configuration: command "ipconfig" was ran in PowerShell. Results showed an IPv4 address and a default gateway.
3. Tested IP Connectivity: Pinged 1.1.1.1 in PowerShell. Replies were recieved.
4. Tested DNS Resolution: command "nslookup github.com" was ran in PowerShell. One IP address was returned.

Analysis: the tests indicated that basic IP connectivity to the tested public destination and DNS resolution for github.com were working during the exercise. These results did not establish that all websites, applications, or internet services were available. No network configurations were made. If a user continued to report a problem, the next step would be to identify the affected website or application, reproduce the issue, record any error message, and investigate the relevent browser, proxy/VPN, firewall, or service.

Notes: private network details and IP addresses have been omitted from this report. 

# Scenario Two: Application Will Not Open
**Reported symptoms:** a user reports that an application does not launch or displays an error.

<ins>Diagnostic Steps</ins>
1. Record the application name and exact error message.
2. Ask whether the issue affecs one application or multiple applications.
3. Check whether the application or multiple applications.
4. Save the user's work before closing or restarting an unresponsive application.
5. Checks for available application updates or approved repair options.
6. Re-test the application and document the result.

<ins>Documentation</ins>
(insert text)

# Scenario Three: User Cannot Sign In 
**Reported symptoms:** a user cannot sign in to their Windows computer or work account

<ins>Diagnostic Steps</ins>
1. Record the displayed error without collecting the user's password
2. Confirm that the user is entering the intended account name.
3. Check keyboard layout, caps lock, and number lock.
4. Determine whether the problem affects a local account or an organization account.
5. For an organizational account, follow the approved identity verification and account recovery process.
6. Retest sign-in after an authorized corrective action.

<ins>Documentation</ins>
(insert text)

# Incident Documentation Template
For each support incident, record:
* Ticket ID: use a fiction identifier for practice.
* Date: record the data of the exercise.
* Reported Issue: summarize the user's symptoms.
* Impact: describe which task or service is affected.
* Diagnostic Steps: list checks performed and their results.
* Resolution: state what fixed the issue or note if it remains unresolved.
* Verification: explain how the result was checked.
* Escalation: record the next action if further support is needed.

# Notes
* A consistent troubleshooting process prevents random unnecessary changes.

* Clear documentation helps another technician continue the investigation without confusion. 

* Security and privacy must be maintained throughout support work.

* Issues should be verified after a fix and escalated when they exceed the technician's authorization or skill level.  
