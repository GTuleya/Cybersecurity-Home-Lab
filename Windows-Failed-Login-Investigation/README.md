# Windows Failed Login Investigation

## Objective

Investigate failed Windows authentication activity using Windows Event Viewer.

## Tools Used

- Windows 11
- Windows Event Viewer

## Lab Setup

I generated controlled authentication failures on my personal Windows lab system and investigated the resulting Windows Security events.

## Event Investigated

Windows Security Event ID 4625 — failed account logon.

## Investigation

I filtered the Windows Security log for Event ID 4625 and identified multiple failed authentication events.

I examined:

- Timestamp
- Account information
- Logon type
- Failure reason
- Status and sub-status codes
- Process information
- Available network information

## Findings

One investigated event contained:

- Event ID: 4625
- Logon Type: 2
- Failure Reason: An Error occurred during Logon
- Status: 0xC000006D
- Sub Status: 0xC0000380
- Process: C:\Windows\System32\svchost.exe
- Result: Audit Failure

The event occurred during controlled testing within my lab environment.

## Conclusion

This project provided hands-on experience locating, filtering, and analyzing Windows authentication events.

I practiced identifying relevant event information and documenting the results of a basic security investigation.

## Skills Practiced

- Windows Event Viewer
- Windows Security Logs
- Authentication monitoring
- Event log analysis
- Security event investigation
- Incident documentation
