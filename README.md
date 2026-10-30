
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


<h3 align="center">Low Priority Tickets</h3> 



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

<h4>2. IT Support Response</h4>

<p align="center">
  <img src="https://i.imgur.com/vXSDo2o.png" width="800">
</p>

## Printer Troubleshooting Walk-Through
<p align="center"><strong>Initial Troubleshooting</strong></p>

<h4>Problem Identification</h4>

<p align="center">
  <img src="https://i.imgur.com/AK9ALHU.png" width="48%">
  <img src="https://i.imgur.com/2cCIaDp.png" width="48%">
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

<h4>Employee Confirmation</h4>

<p align="center">
  <img src="https://i.imgur.com/0dMbP4V.png" width="1000">
</p>

<p align="center"><strong>Resolution Confirmed</strong></p>

## End Of Printer Troubleshooting Walk-Through
<h4>Ticket Closure</h4>

<p align="center">
  <img src="images/003-ticket-closed.png" width="800">
</p>

<p align="center"><strong>Ticket Closed</strong></p>




### Medium Priority Tickets

#### Ticket HD-001: Password Reset

#### Ticket HD-002: Account Locked Out

#### Ticket HD-004: Cannot Access Shared Folder



### High Priority Tickets

#### Ticket HD-005: Domain Connectivity / DNS Failure

#### Ticket HD-006: Tier 2 Escalation

## What I Learned

This section will summarize the ticket management, troubleshooting, communication, documentation, and escalation skills gained after completing all six scenarios.
