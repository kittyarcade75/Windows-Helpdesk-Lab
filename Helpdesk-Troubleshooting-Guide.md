# Purpose 
This guide will document a repeatable process for diagnosing common Windows 11 support issues. It will focus on gatherin symptoms, performing safe checks, documenting findings, and escelating problems when necessary. 

## Lab Enviornment
Operating System: Windows 11 

Tools: Windows settings, Windows PowerShell, built-in Windows troubleshooting tools

Environment: personal practice lab 

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
Reported symptoms: a user reports that their Windows computer cannot access the internet 

Diagnostic Steps
1. Check whether Wi-Fi is enabled and the computer is connected to the expected network.
2. Run the command "ipconfig /all" in PowerShell to inspect network configuration.
3. Run the command "1.1.1.1" in PowerShell to test connectivity to an external IP address.
4. Run the command "nslookup (insert domain)" in PowerShell to test DNS resolution.
5. Compare the results to identify the likely area of failure.

Documentation
(insert text)

# Scenario Two: Application Will Not Open
Reported symptoms: a user reports that an application does not launch or displays an error.

Diagnostic Steps
1. Record the application name and exact error message.
2. Ask whether the issue affecs one application or multiple applications.
3. Check whether the application or multiple applications.
4. Save the user's work before closing or restarting an unresponsive application.
5. Checks for available application updates or approved repair options.
6. Re-test the application and document the result.


Documentation
(insert text)

# Scenario Three: User Cannot Sign In 
