## Step-by-Step Instructions

Step 1: Open Event Viewer

1. Click the Windows Start button.

2. Search for Event Viewer.

3. Open the application.

4. Wait for the Event Viewer window to load.

Step 2: Navigate to Security Logs

1. Locate the Windows Logs section on the left.

2. Click the arrow beside Windows Logs.

3. Select Security.

4. Review the events displayed.

What this does:

Windows Event Viewer records activity occurring on your computer. Security logs can contain information about authentication attempts and other security-related events.

Screenshot 1: Save a screenshot of the Security log.

Step 3: Look for Failed Login Attempts

1. Locate the Filter Current Log option.

2. Enter Event ID: 4625

3. Click OK.

4. Review any matching events.

What this means:

Event ID 4625 represents a failed login attempt.

Repeated failures may deserve investigation, but they do not automatically mean an attack occurred.

Screenshot 2: Save a screenshot showing the filtered results, if available.

Step 4: Look for Successful Logins

1. Select Filter Current Log again.

2. Enter: 4624

3. Click OK.

4. Review the matching events.

What this means:

Event ID 4624 represents a successful login.

Security professionals examine successful logins alongside other activity to determine whether access was expected.

Screenshot 3: Save a screenshot showing successful login events, if available.

Step 5: Investigate an Event

Double-click an event to examine its details.

Look for information such as:

- Account name

- Time of the event

- Logon type

- Source network information, if available

- Failure reason, when applicable

Do not publish personal usernames, computer names, IP addresses, or other private information in your public repository.

Step 6: Document Your Findings

Answer these questions:

1. What is Windows Event Viewer? It is a built-in Windows diagnostic tool that records events happening on your computer. It helps you understands what Windows, applications, and hardware are doing and troubleshoot problems when something goes wrong.

2. What does Event ID 4625 represent? It means someone or something attempted to sign in to a Windows computer or account, but Windows rejected the login. 

3. What does Event ID 4624 represent? It means a user account successfully authenticated to a Windows computer or system.

4. Why might repeated failed login attempts be suspicious? Repeated failed login attempts can be suspicious because they may indicate that someone is trying to gain unauthorized access to a computer or user account. 

5. Why should an analyst investigate successful logins after repeated failures? It could indicate that an attacker eventually guessed or obtained the correct password and gained unauthorized access.

If your computer does not contain useful examples, use fictional training logs and clearly identify them as simulated data.




Explain whether you found failed logins, successful logins, both, or neither.

Conclusion

This lab introduced basic security monitoring and demonstrated how Windows authentication logs can help an analyst investigate potentially suspicious login activity.
