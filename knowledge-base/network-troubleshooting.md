# Network Connectivity Troubleshooting

## Overview

This guide provides troubleshooting procedures for common network connectivity problems. It helps IT support technicians identify connection issues, investigate possible causes and restore access to network resources.

## 1. Common Symptoms

Users experiencing network problems may report:

- Unable to access the internet.
- Unable to connect to shared network resources.
- Network connection displays as disconnected.
- Limited or no network access.
- Applications cannot reach network services.
- Intermittent network connectivity.

## 2. Possible Causes

Common causes include:

- Loose or disconnected network cables.
- Incorrect IP address configuration.
- Incorrect default gateway or DNS settings.
- DHCP service problems.
- Network adapter issues.
- Wireless connectivity problems.
- Network equipment or service interruptions.

## 3. Troubleshooting Procedure

### Step 1: Identify the Scope of the Problem

- Determine whether the issue affects one user or multiple users.
- Confirm whether the computer uses Ethernet or Wi-Fi.
- Check the network connection status.
- For Ethernet connections, inspect the cable and connection indicators.
- Establish whether other employees can access network resources.

### Step 2: Check IP Configuration

On Windows, open Command Prompt and run:

```cmd
ipconfig /all
```

Review the following information:

- IPv4 address.
- Subnet mask.
- Default gateway.
- DNS server addresses.

Check whether the computer has received an appropriate IP address for its network.

An address beginning with `169.254` may indicate that the computer has not received an IP address from a DHCP server.

### Step 3: Test Network Connectivity

Use Command Prompt to test connectivity.

Test the local network configuration:

```cmd
ipconfig
```

Test communication with the default gateway:

```cmd
ping <default-gateway>
```

Replace `<default-gateway>` with the actual gateway address displayed by `ipconfig`.

A failed ping does not always mean the network is unavailable, as some devices block ping requests.

### Step 4: Investigate DNS Issues

DNS translates domain names into IP addresses.

Use the following command to investigate name resolution:

```cmd
nslookup example.com
```

Review whether the hostname resolves successfully.

If IP connectivity works but names cannot be resolved, investigate the configured DNS server and escalate DNS service issues when necessary.

### Step 5: Check DHCP Configuration

If the computer has an incorrect or missing IP configuration:

- Confirm that the network adapter is enabled.
- Check whether the computer is configured to obtain an IP address automatically.
- Confirm that the DHCP service is available.
- If authorised and the adapter uses DHCP, renew its configuration:

```cmd
ipconfig /release
ipconfig /renew
```

Avoid changing static IP configurations without approval.

### Step 6: Apply the Appropriate Resolution

Depending on the investigation:

- Reconnect or replace a faulty network cable.
- Correct IP address settings.
- Restore DHCP configuration.
- Correct gateway or DNS settings.
- Reconnect the computer to the appropriate network.
- Escalate network infrastructure problems when necessary.

## 4. Verification

After applying the corrective action:

- Confirm that the computer has a valid IP configuration.
- Test connectivity to the default gateway.
- Verify DNS name resolution where applicable.
- Test access to the internet and required network resources.
- Ask the user to confirm that normal connectivity has been restored.

## 5. Related Portfolio Incident

**Incident INC003 - Network Connectivity Issue**

The simulated incident demonstrated how an incorrect IP configuration can prevent an employee from accessing network resources. The issue was addressed by restoring the appropriate DHCP configuration.

[View Incident 003](../tickets/incident-003-network.md)

## 6. Escalation

Escalate the issue to a senior technician or network administrator if:

- Multiple employees experience connectivity problems.
- Network equipment appears unavailable.
- DHCP or DNS services are not functioning.
- Connectivity remains unavailable after standard troubleshooting.
- The issue requires changes to network infrastructure.

---

*Note: This knowledge-base article is prepared for practical IT support learning.*
