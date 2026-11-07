# Outlook Connectivity Troubleshooting

## Overview

This guide provides troubleshooting procedures for common Microsoft Outlook desktop connectivity problems. It is intended to help IT support technicians identify possible causes and restore normal email access.

## 1. Common Symptoms

Users experiencing Outlook connectivity problems may report:

- Outlook displays a Disconnected status.
- Outlook cannot connect to the mail server.
- Emails cannot be sent or received.
- Outlook displays connection error messages.
- Outlook works in the browser but not in the desktop application.

## 2. Possible Causes

Common causes include:

- Internet connectivity problems.
- Incorrect account or connection settings.
- Microsoft 365 service interruptions.
- Outdated Outlook applications.
- Corrupted Outlook profiles.
- Conflicts caused by third-party add-ins.

## 3. Troubleshooting Procedure

### Step 1: Check Internet Connectivity

- Confirm that the computer has an active internet connection.
- Open a web browser and access a trusted website.
- Check whether other applications can connect to the internet.

### Step 2: Test Outlook on the Web

- Open Outlook on the web.
- Sign in using the user's Microsoft 365 account.
- Confirm whether emails can be accessed.

If Outlook on the web works but the desktop application does not, investigate the desktop application further.

### Step 3: Check Outlook Connection Status

- Open Outlook.
- Review the connection status displayed at the bottom of the application window.
- Check for statuses such as Disconnected or Trying to connect.
- Record any displayed error messages.

### Step 4: Check Microsoft 365 Applications

- Confirm whether other Microsoft 365 applications are functioning.
- Check whether the issue affects only Outlook or multiple services.
- Consider whether the problem may be related to a wider service interruption.

### Step 5: Investigate Add-in Conflicts

For classic Outlook:

- Close Outlook.
- Open Outlook in Safe Mode.
- Check whether the connectivity problem persists.
- If Outlook works normally in Safe Mode, investigate installed add-ins.
- Disable suspected add-ins one at a time, following organisational procedures.
- Restart Outlook normally after each change to identify the problematic add-in.

Only disable approved add-ins, and document any configuration changes.

### Step 6: Apply the Appropriate Resolution

Depending on the findings:

- Restore internet connectivity if required.
- Correct relevant Outlook settings.
- Update Microsoft 365 applications.
- Investigate and resolve problematic add-ins.
- Escalate account, service or profile issues when necessary.

## 4. Verification

After applying a corrective action:

- Restart Outlook.
- Confirm that the application connects successfully.
- Test sending and receiving emails.
- Confirm that no connection errors remain.
- Ask the user to confirm that normal email access has been restored.

## 5. Related Project Incident

**Incident 001 – Outlook Connectivity Issue**

The simulated incident demonstrated how a third-party CRM add-in could interfere with Outlook connectivity and how controlled add-in testing could help identify the cause.

[View Incident 001](../tickets/incident-001-outlook.md)

## 6. Escalation

Escalate the issue to the appropriate Microsoft 365 administrator or senior technician if:

- Multiple users experience the same problem.
- Account authentication problems persist.
- Microsoft 365 services are unavailable.
- The issue remains unresolved after standard troubleshooting.

---

*Note: This knowledge-base article is prepared for practical IT support learning.*
