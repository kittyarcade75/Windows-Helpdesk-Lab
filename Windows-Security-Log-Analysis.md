# Objective
This lab is to help me practice reviewing Windows security events, interpret logon activity, correlate nearby events, and document findings using a structured SOC analyst approach.

# Lab Enviornment
* Operating System: Windows 11
* Tool: Windows event viewer

# Investigation Steps
1. Locate the security log: open the event viewer and navigate to Windows Logs -> Security. Confirm the security events are available for review.
2. Filter Successful Logon Events: Filter the security log for event ID and select an event for inspection.
3. Review Logon Type: identify the logon type
4. Check Nearby Events: review surrounding security log entries that include different event IDs.

# Investigation Guide
<ins>Event IDs</ins>
4624 = succesful logon

<ins>Logon Types</ins>
5 = service logon (Windows and application service operations)
