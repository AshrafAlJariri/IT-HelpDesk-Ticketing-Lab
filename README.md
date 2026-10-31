
# IT-HelpDesk-Ticketing-Lab

A hands-on IT Help Desk lab demonstrating ticket management, troubleshooting, issue resolution, and escalation using Spiceworks Cloud Help Desk, Active Directory, and Windows administration tools.

## Description

I created this lab to simulate real-world IT Help Desk operations using Spiceworks Cloud Help Desk. I practiced receiving employee support requests, assigning ticket priorities, communicating with users, troubleshooting technical issues, documenting resolutions, and escalating complex problems when necessary.

## Tools and Technologies Used

- Spiceworks Cloud Help Desk
- Active Directory Users and Computers (ADUC)
- Windows Server 2025
- Windows 11 Pro
- Windows PowerShell
- Remote Desktop Connection (RDP)
- Microsoft Azure

## Help Desk Ticket Scenarios

| Ticket | Issue | Priority |
|--------|-------|----------|
| HD-001 | Printer Not Working | Low |
| HD-002 | Password Reset | Medium |
| HD-003 | Account Locked Out | Medium |
| HD-004 | Cannot Access Shared Folder | Medium |
| HD-005 | Domain Connectivity / DNS Failure | High |
| HD-006 | Tier 2 Escalation | High |

## Lab Walk-Through


<h3 align="center">(Low Priority Tickets)</h3> 



<h3>HD-003: Printer Not Working</h3>


<p align="center">
  <strong>Ticket Creation:</strong> John Smith submitted a support request after experiencing printing issues on his Windows 11 workstation. The ticket was assigned Low priority.
</p>

<p align="center">
  <img src="https://i.imgur.com/AfT9CWM.png" width="800">
</p>

<p align="center"><strong>Initial Support Request</strong></p>

<h4>IT Support Response</h4>

<p align="center">
  <img src="https://i.imgur.com/hOmWwK8.png" width="800">
</p>

<h4>John Response</h4>

<p align="center">
  <img src="https://i.imgur.com/vXSDo2o.png" width="800">
</p>

## Printer Troubleshooting Walk-Through
<p align="center"><strong>Initial Troubleshooting</strong></p>

<h4>Problem Identification</h4>

<p align="center">
  <img src="https://i.imgur.com/AK9ALHU.png" width="48%">
  
</p>
<p align="center">
  <strong>Problem Identification:</strong> I attempted to print a test page using Microsoft Print to PDF but received error 0x000006ba, indicating that the Print Spooler service was not running.
</p>

<p align="center"><strong>Print Spooler Service Restoration</strong></p>

<h4>Troubleshooting and Resolution</h4>

<p align="center">
  <img src="https://i.imgur.com/TivuJon.jpeg" width="100%">
</p>
<p align="center">
  <strong>Print Spooler Service Restoration:</strong> I opened the Windows Services application and located the Print Spooler service. After discovering that the service was not running, I changed its startup type to Automatic and started the service to restore printing functionality.
</p>


<p align="center"><strong>Service Configuration | Service Restored</strong></p>

<h4>Resolution Verification</h4>

<p align="center">
   <img src="https://i.imgur.com/QeLayha.png" width="70%">
  </p>
<p align="center">
  <strong>Resolution Verification:</strong> After changing the Print Spooler startup type to Automatic and starting the service, I returned to the Windows Services application and verified that the Print Spooler status displayed "Running," confirming that the service had been successfully restored.
</p>

 

<p align="center"><strong>Print Test Successful</strong></p>

<h4>Print Test Verification</h4>

<p align="center">
  <img src="https://i.imgur.com/0dMbP4V.png" width="1000">
</p>
<p align="center">
  <strong>Print Test Verification:</strong> After confirming the Print Spooler service was running, I successfully generated and saved a Windows Printer Test Page using Microsoft Print to PDF. I opened the saved PDF to verify that the test page was created correctly, confirming that PDF printing functionality was restored.
</p>


## End Of Printer Troubleshooting Walk-Through
<p align="center"><strong>Resolution Confirmed</strong></p>

<p align="center">
  <img src="https://i.imgur.com/imWOkS2.png" width="80">
</p>

<p align="center">
  <strong>Resolution Confirmation:</strong> I informed John Smith that I restored the Print Spooler service and successfully tested Microsoft Print to PDF. John confirmed that he was able to print documents again without any issues.
</p>
<h4> Ticket Documentation</h4>

<p align="center">
  <img src="https://i.imgur.com/8P5w52s.png" width="800">
</p>

<p align="center">
  <strong>Ticket Documentation:</strong> I documented the reported issue, troubleshooting steps, root cause, resolution, verification results, and employee confirmation in a private Spiceworks internal note before closing the ticket.
</p>

<h4>Ticket Closed</h4>

<p align="center">
  <img src="https://i.imgur.com/ljL5E9B.png" width="800">
</p>
<p align="center">
  <strong>Ticket Closed:</strong> After successfully resolving the printer issue, verifying that printing functionality was restored, and receiving confirmation from John Smith, I documented the troubleshooting steps and resolution in an internal note. I then closed the ticket in Spiceworks.
</p>


<h3 align="center">(Medium Priority Tickets)</h3> 

#### Ticket HD-001: Password Reset

<p align="center">
  <strong>Ticket Creation:</strong> John Smith submitted a support request after forgetting his Windows login password and being unable to access his workstation. The ticket was assigned Medium priority.
</p>

<p align="center">
  <img src="https://i.imgur.com/xCaIS9s.png" width="800">
</p>

<p align="center"><strong>Initial Support Request</strong></p>

<h4>IT Support Response</h4>

<p align="center">
  <img src="https://i.imgur.com/iI4ZfO6.png" width="800">
</p>

<h4>John Response</h4>

<p align="center">
  <img src="https://i.imgur.com/M7Dl2b5.png" width="800">
</p>


## Password Reset Troubleshooting Walk-Through

<p align="center"><strong>Initial Troubleshooting</strong></p>

<h4>Problem Identification</h4>

<p align="center">
  <img src="https://i.imgur.com/W5cxYFl.png" width="70%">
</p>
<p align="center">
  <strong>Problem Identification:</strong> I attempted to sign in to John Smith's Windows 11 workstation and received an incorrect password error, confirming that the existing credentials were not working.
</p>

<p align="center"><strong>Windows Login Failure</strong></p>


<h4>Active Directory Password Reset</h4>

<p align="center">
  <img src="https://i.imgur.com/00b7xUS.png" width="800%">

</p>

<p align="center">
  <strong>Active Directory Password Reset:</strong> I opened Active Directory Users and Computers, located John Smith's account in the IT organizational unit, and reset his password. I selected "User must change password at next logon" to require John to create a new password when signing in. Active Directory confirmed that the password was successfully changed.
</p>

<p align="center"><strong>Password Reset Configuration | Password Reset Successful</strong></p>


<h4>Password Change Required</h4>
<p align="center">
  <img src="https://i.imgur.com/Ap40uSi.png" width="70%">
</p>

<p align="center">
  <strong>Password Change Verification:</strong> After entering the temporary password, Windows prompted John Smith to change his password before signing in. I completed the required password change process, and Windows confirmed that the new password was successfully set.
</p>

<p align="center"><strong>Password Change Required | Password Changed Successfully</strong></p>


<h4>Entering New Password</h4>

<p align="center">
  <img src="https://i.imgur.com/OaUrsgN.png" width="80%">
</p>
<p align="center">
  <strong>Password Change Successful:</strong> I entered the temporary password and configured a new password for John Smith's domain account. Windows displayed the message "Your password has been changed," confirming that the required password update was completed successfully.
</p>
<p align="center">
  <strong>New Password Configuration | Password Change Confirmed</strong>
</p>

<h4>Domain Login Verification</h4>
  <p align="center">
  <img src="https://i.imgur.com/FdAIutf.jpeg" width="800%">
</p>
<p align="center">
  <strong>Domain Login Verification:</strong> After changing the password, I successfully signed in to the Windows 11 workstation using John Smith's updated credentials. I then opened Command Prompt and executed the whoami command, which returned CORP\john.smith, verifying that the correct domain user account was signed in.
</p>
<p align="center">
  <strong>Successful Windows Login | Domain Account Verification</strong>
</p>


## End Of Password Reset Troubleshooting Walk-Through

<p align="center"><strong>Resolution Confirmed</strong></p>

<p align="center">
  <img src="https://i.imgur.com/zCq3iPF.png" width="70%">
</p>

<p align="center">
  <strong>Resolution Confirmation:</strong> I informed John Smith that his Active Directory password had been reset and the new password was working successfully. John confirmed that he could access his Windows workstation again.
</p>


<h4>Ticket Documentation</h4>

<p align="center">
  <img src="YOUR-INTERNAL-NOTE-IMAGE-URL" width="800">
</p>

<p align="center">
  <strong>Ticket Documentation:</strong> I documented the reported login issue, troubleshooting steps, Active Directory password reset, required password change, and successful login verification in a private Spiceworks internal note before closing the ticket.
</p>


<h4>Ticket Closed</h4>

<p align="center">
  <img src="https://i.imgur.com/zCq3iPF.png" width="800">
</p>

<p align="center">
  <strong>Ticket Closed:</strong> After successfully resetting John Smith's password, verifying that he could sign in to his domain account, and receiving employee confirmation, I documented the resolution in an internal note and closed the ticket in Spiceworks.
</p>







#### Ticket HD-002: Account Locked Out

#### Ticket HD-004: Cannot Access Shared Folder



### High Priority Tickets

#### Ticket HD-005: Domain Connectivity / DNS Failure

#### Ticket HD-006: Tier 2 Escalation

## What I Learned

This section will summarize the ticket management, troubleshooting, communication, documentation, and escalation skills gained after completing all six scenarios.
