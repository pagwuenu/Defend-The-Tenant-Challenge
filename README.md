# Defend-The-Tenant-Challenge
Microsoft 365 tenant security hardening submission for Microsoft Innovation Studio's Defend the Tenant competition.
Defend the Tenant - Microsoft 365 Security Hardening

Microsoft Innovation Studio competition entry demonstrating end-to-end Microsoft 365 tenant security hardening for a 100-user SMB organization with Microsoft 365 E7 licensing.

Scenario

A small business with 100 users and 2 administrators requires a comprehensive identity and access security baseline. All controls are deployed using Microsoft Entra ID Conditional Access policies, Identity Protection, and Microsoft Teams governance settings.

Security Controls Implemented

Conditional Access Policies

CA001 - Phishing-resistant MFA for all administrative roles using FIDO2/passkey authentication strength
CA002 - MFA required for all users across all cloud applications
CA003 - Block legacy authentication (Exchange ActiveSync and other legacy clients) for all users
CA004 - Risk-based sign-in policy requiring MFA with every-time reauthentication on medium and high sign-in risk
CA005 - User risk remediation requiring MFA and password change with every-time reauthentication on high user risk

Identity and Access Controls

User consent to applications accessing company data disabled; Admin Consent Workflow enabled
Self-service password reset enabled for all users

Microsoft Teams Governance

Only invited users automatically admitted to meetings
Presenter role restricted to organizer with user override
Anonymous users blocked from joining meetings
Assessment Results

All 10 security recommendations scored IMPLEMENTED by the automated assessment script. See hardening-results.txt for the full output.

Tenant Details
Tenant ID: 51015d4b-a764-4585-993a-abfc28bee313
Licensing: Microsoft 365 E7 (includes Entra ID P2 for Identity Protection)
Users: 100 standard users, 2 administrators, 2 break-glass accounts
Tools Used
Microsoft Graph PowerShell SDK
Microsoft Entra admin center
Microsoft Teams admin center
