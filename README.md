# Microsoft 365 New Tenant Security Baseline

> CIS-aligned implementation checklist derived from the **CIS Microsoft 365 Foundations Benchmark v7.0.0**.

## Purpose

Use this repository checklist to build, validate, and document the security baseline for a new Microsoft 365 tenant. The deployable baseline below contains the benchmark controls assigned to a **Level 1** profile. Level 2 recommendations are retained in a separate enhanced-hardening register.

## Important notice

- This README is an implementation aid and does not replace the authoritative CIS benchmark.
- Review current Microsoft licensing, portal paths, service behavior, and customer requirements before enforcement.
- Obtain the benchmark directly from CIS for the complete rationale, impact, default values, references, and CIS Controls mappings.
- Do not publish or redistribute the source CIS PDF unless your CIS license permits it.

## Tenant information

- **Customer / tenant:**
- **Tenant ID:**
- **Implementation owner:**
- **Review date:**
- **Target license profile:**

## Deployment rules

- [ ] Create and test emergency access accounts before Conditional Access enforcement.
- [ ] Use dedicated cloud-only administrative accounts and least privilege.
- [ ] Pilot user-impacting policies or use Report-only mode, validate, and then enforce.
- [ ] Document every exclusion with an owner, business reason, compensating control, and expiration date.
- [ ] Capture dated evidence for every validation step.

## Recommended implementation sequence

1. Emergency access, cloud-only administration, and privileged-role governance.
2. Authentication methods, MFA, Conditional Access, risk policies, and device registration.
3. Exchange Online Protection and Microsoft Defender for Office 365.
4. Purview auditing, DLP, and sensitivity labels.
5. SharePoint, OneDrive, Teams, Power Platform, and Fabric sharing restrictions.
6. Evidence collection, exception approval, and recurring reviews.

## Baseline scope

- **Level 1 controls:** 114
- **Enhanced controls listed for evaluation:** 46

## Level 1 control register

| ID | Control | Profiles | Status |
|---|---|---|---|
| 1.1.1 | Ensure Administrative accounts are cloud-only (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 1.1.2 | Ensure two emergency access accounts have been defined (Manual) | E3 Level 1, E5 Level 1 | ☐ |
| 1.1.3 | Ensure that between two and four global admins are designated (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 1.1.4 | Ensure administrative accounts use licenses with a reduced application footprint (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 1.2.2 | Ensure sign-in to shared mailboxes is blocked (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 1.3.1 | Ensure the 'Password expiration policy' is set to 'Set passwords to never expire (recommended)' (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 1.3.4 | Ensure 'User owned apps and services' is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 1.3.5 | Ensure internal phishing protection for Forms is enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 1.3.9 | Ensure shared bookings pages are restricted to select users (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.2 | Ensure the Common Attachment Types Filter is enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.3 | Ensure notifications for internal users sending malware is Enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.6 | Ensure Exchange Online Spam Policies are set to notify administrators (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.8 | Ensure that SPF records are published for all Exchange Domains (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.9 | Ensure that DKIM is enabled for all Exchange Online Domains (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.10 | Ensure DMARC records for all Exchange Online domains are published (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.12 | Ensure the connection filter IP allow list is not used (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.13 | Ensure the connection filter safe list is off (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.14 | Ensure inbound anti-spam policies do not contain allowed domains (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.1.15 | Ensure outbound anti-spam message limits are in place (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 2.2.1 | Ensure emergency access account activity is monitored (Manual) | E5 Level 1 | ☐ |
| 2.4.1 | Ensure Priority account protection is enabled and configured (Automated) | E5 Level 1 | ☐ |
| 2.4.2 | Ensure Priority accounts have 'Strict protection' presets applied (Automated) | E5 Level 1 | ☐ |
| 2.4.4 | Ensure Zero-hour auto purge for Microsoft Teams is on (Automated) | E5 Level 1 | ☐ |
| 2.4.5 | Ensure 'AIR' remediation is enabled (Manual) | E5 Level 1 | ☐ |
| 3.1.1 | Ensure Microsoft 365 audit log search is Enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 3.2.1 | Ensure DLP policies are enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 3.2.2 | Ensure DLP policies are enabled for Microsoft Teams (Automated) | E5 Level 1 | ☐ |
| 3.2.3 | Ensure DLP policies are published for Copilot users (Automated) | E5 Level 1 | ☐ |
| 3.3.1 | Ensure Information Protection sensitivity label policies are published (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 4.1 | Ensure devices without a compliance policy are marked 'not compliant' (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 4.2 | Ensure device enrollment for personally owned devices is blocked by default (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.2.1 | Ensure 'Per-user MFA' is disabled (Manual) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.2.2 | Ensure users cannot register applications (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.2.3 | Ensure 'Restrict non-admin users from creating tenants' is set to 'Yes' (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.2.4 | Ensure access to the Entra admin center is restricted (Manual) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.3.1 | Ensure users cannot create security groups (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.3.3 | Ensure that 'Owners can manage group membership requests in My Groups' is set to 'No' (Manual) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.4.2 | Ensure the maximum number of devices per user is limited (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.4.3 | Ensure the GA role is not added as a local administrator during Entra join (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.4.4 | Ensure local administrator assignment is limited during Entra join (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.4.5 | Ensure Local Administrator Password Solution is enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.5.2 | Ensure the admin consent workflow is enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.5.4 | Ensure password lifetime for applications does not exceed 180 days (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.5.5 | Ensure new application passwords are system-generated (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.5.6 | Ensure maximum certificate lifetime for applications does not exceed 180 days (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.6.2 | Ensure that guest user access is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.1.8.1 | Ensure that password hash sync is enabled for hybrid deployments (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.1 | Ensure multifactor authentication is enabled for all users in administrative roles (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.2 | Ensure multifactor authentication is enabled for all users (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.3 | Enable Conditional Access policies to block legacy authentication (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.4 | Ensure Sign-in frequency is enabled and browser sessions are not persistent for Administrative users (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.6 | Enable Identity Protection user risk policies (Automated) | E5 Level 1 | ☐ |
| 5.2.2.7 | Enable Identity Protection sign-in risk policies (Automated) | E5 Level 1 | ☐ |
| 5.2.2.9 | Ensure a managed device is required for authentication (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.10 | Ensure a managed device is required to register security information (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.11 | Ensure sign-in frequency for Intune Enrollment is set to 'Every time' (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.12 | Ensure the device code sign-in flow is blocked (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.13 | Ensure that periodic reauthentication is required for all users (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.2.17 | Ensure authentication transfer is blocked (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.3.1 | Ensure Microsoft Authenticator is configured to protect against MFA fatigue (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.3.2 | Ensure custom banned passwords lists are used (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.3.3 | Ensure password protection is enabled for on-prem Active Directory (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.3.4 | Ensure all member users are 'MFA capable' (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.3.5 | Ensure weak authentication methods are disabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.3.6 | Ensure system-preferred multifactor authentication is enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.3.8 | Ensure that Account 'Lockout threshold' is '10' or less (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.3.9 | Ensure that Account 'Lockout duration in seconds' is at least 60 seconds (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.3.10 | Ensure Microsoft Authenticator on companion applications is disabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.4.1 | Ensure 'Self service password reset enabled' is set to 'All' (Manual) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.4.3 | Ensure SSPR registration and authentication re- confirmation are required (Manual) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.4.4 | Ensure that users are notified on password resets (Manual) | E3 Level 1, E5 Level 1 | ☐ |
| 5.2.4.5 | Ensure all admins are notified when other admins reset their password (Manual) | E3 Level 1, E5 Level 1 | ☐ |
| 5.3.2 | Ensure 'Access reviews' for guest users are configured (Automated) | E5 Level 1 | ☐ |
| 5.3.3 | Ensure 'Access reviews' for privileged roles are configured (Automated) | E5 Level 1 | ☐ |
| 5.3.4 | Ensure approval is required for Global Administrator role activation (Automated) | E5 Level 1 | ☐ |
| 5.3.5 | Ensure approval is required for Privileged Role Administrator activation (Automated) | E5 Level 1 | ☐ |
| 6.1.1 | Ensure 'AuditDisabled' organizationally is set to 'False' (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 6.1.2 | Ensure mailbox audit actions are configured (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 6.1.3 | Ensure 'AuditBypassEnabled' is not enabled on mailboxes (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 6.2.1 | Ensure all forms of mail forwarding are blocked and/or disabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 6.2.2 | Ensure mail transport rules do not whitelist specific domains (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 6.2.3 | Ensure email from external senders is identified (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 6.3.2 | Ensure the ability to add personal email accounts and calendars is disabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 6.5.1 | Ensure modern authentication for Exchange Online is enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 6.5.2 | Ensure MailTips are enabled for end users (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 6.5.4 | Ensure SMTP AUTH is disabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 7.2.1 | Ensure modern authentication for SharePoint applications is required (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 7.2.2 | Ensure SharePoint and OneDrive integration with Azure AD B2B is enabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 7.2.3 | Ensure external content sharing is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 7.2.7 | Ensure link sharing is restricted in SharePoint and OneDrive (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 7.2.9 | Ensure guest access to a site or OneDrive will expire automatically (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 7.2.10 | Ensure reauthentication with verification code is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 7.2.11 | Ensure the SharePoint default sharing link permission is set (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 8.1.2 | Ensure users can't send emails to a channel email address (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 8.2.2 | Ensure communication with unmanaged Teams users is disabled (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 8.2.3 | Ensure external Teams users cannot initiate conversations (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 8.2.4 | Ensure the organization cannot communicate with accounts in trial Teams tenants (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 8.4.1 | Ensure app permission policies are configured (Manual) | E3 Level 1, E5 Level 1 | ☐ |
| 8.5.2 | Ensure anonymous users and dial-in callers can't start a meeting (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 8.5.3 | Ensure only people in my org can bypass the lobby (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 8.5.4 | Ensure users dialing in can't bypass the lobby (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 8.5.7 | Ensure external participants can't give or request control (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 8.6.1 | Ensure users can report security concerns in Teams (Automated) | E5 Level 1 | ☐ |
| 9.1.1 | Ensure guest user access is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.2 | Ensure external user invitations are restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.3 | Ensure guest access to content is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.4 | Ensure 'Publish to web' is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.6 | Ensure 'Allow users to apply sensitivity labels for content' is 'Enabled' (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.7 | Ensure shareable links are restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.8 | Ensure enabling of external data sharing is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.9 | Ensure 'Block ResourceKey Authentication' is 'Enabled' (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.10 | Ensure access to APIs by service principals is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.11 | Ensure service principals cannot create and use profiles (Automated) | E3 Level 1, E5 Level 1 | ☐ |
| 9.1.12 | Ensure service principals ability to create workspaces, connections and deployment pipelines is restricted (Automated) | E3 Level 1, E5 Level 1 | ☐ |

## 1. Administration and organization settings

### 1.1.1 Ensure Administrative accounts are cloud-only (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Administrative accounts are special privileged accounts that could have varying levels of access to data, users, and settings.

#### Configuration

1. [ ] Remediation will require first identifying the privileged accounts that are synced from on- premises and then creating a new cloud-only account for that user. Once a replacement account is established, the hybrid account should have its role reduced to that of a non- privileged user or removed depending on the need.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Identity > Users and select All users.
3. [ ] To the right of the search box click the Add filter button.
4. [ ] Add the On-premises sync enabled filter with the value set to Yes and click Apply.
5. [ ] Verify that no user accounts in administrative roles are present in the filtered list.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 1.1.2 Ensure two emergency access accounts have been defined (Manual)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Emergency access or "break glass" accounts are limited for emergency scenarios where normal administrative accounts are unavailable.

#### Configuration

1. [ ] Step 1 - Create two emergency access accounts:
2. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com
3. [ ] Expand Users > Active Users
4. [ ] Click Add user and create a new user with this criteria: o Name the account in a way that does NOT identify it with a particular person. o Assign the account to the default .onmicrosoft.com domain and not the organization's. o The password must be at least 16 characters and generated randomly. o Do not assign a license. o Assign the user the Global Administrator role.
5. [ ] Repeat the above steps for the second account. Step 2 - Exclude at least one account from conditional access policies:
6. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
7. [ ] Expand Protection > Conditional Access.
8. [ ] Inspect the conditional access policies.
9. [ ] For each rule add an exclusion for at least one of the emergency access accounts.
10. [ ] Users > Exclude > Users and groups and select one emergency access account. Step 3 - Ensure the necessary procedures and policies are in place:
11. [ ] In order for accounts to be effectively used in a break glass situation the proper policies and procedures must be authorized and distributed by senior management.
12. [ ] FIDO2 Security Keys should be locked in a secure separate fireproof location.

#### Validation and evidence

1. [ ] Step 1 - Ensure a policy and procedure is in place at the organization:
2. [ ] In order for accounts to be effectively used in a break-glass situation the proper policies and procedures must be authorized and distributed by senior management.
3. [ ] FIDO2 Security Keys should be locked in a secure separate fireproof location.
4. [ ] Passwords should be at least 16 characters, randomly generated and MAY be separated in multiple pieces to be joined in case of an emergency. Step 2 - Ensure two emergency access accounts are defined:
5. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com
6. [ ] Expand Users > Active Users
7. [ ] Inspect the designated emergency access accounts and ensure the following: o The accounts are named correctly, and do NOT identify with a particular person. o The accounts use the default .onmicrosoft.com domain and not the organization's. o The accounts are cloud-only. o The accounts are unlicensed. o The accounts are not disabled or Sign-in blocked. o The accounts are assigned the Global Administrator directory role. Step 3 - Ensure at least one account is excluded from all conditional access rules:
8. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
9. [ ] Expand Protection > Conditional Access.
10. [ ] Inspect the conditional access rules.
11. [ ] Ensure one of the emergency access accounts is excluded from all rules. Warning: As of 10/15/2024 MFA is required for all users including Break Glass Accounts. It is recommended to update these accounts to use passkey (FIDO2) or configure certificate-based authentication for MFA. Both methods satisfy the MFA requirement.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 1.1.3 Ensure that between two and four global admins are designated (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Between two and four global administrators should be designated in the tenant.

#### Configuration

1. [ ] Navigate to the Microsoft 365 admin center https://admin.microsoft.com
2. [ ] Select Users > Active Users.
3. [ ] In the Search field enter the name of the user to be made a Global Administrator.
4. [ ] To create a new Global Admin:
5. [ ] Select the user's name.
6. [ ] A window will appear to the right.
7. [ ] Select Manage roles.
8. [ ] Select Admin center access.
9. [ ] Check Global Administrator.
10. [ ] Click Save changes.
11. [ ] To remove a Global Admin:
12. [ ] In the Search field, enter the name of the user to be removed.

#### Validation and evidence

1. [ ] Navigate to the Microsoft 365 admin center https://admin.microsoft.com
2. [ ] Select Roles > Role assignments.
3. [ ] Select the Global Administrator role from the list and click on Assigned.
4. [ ] Review the list of Global Administrators. o If there are groups present, then inspect each group and its members. o Take note of the total number of Global Administrators in and outside of groups.
5. [ ] Verify the number of Global Administrators is between two and four.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 1.1.4 Ensure administrative accounts use licenses with a reduced application footprint (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Administrative accounts are special privileged accounts that could have varying levels of access to data, users, and settings.

#### Configuration

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Users > Active users.
3. [ ] Click Add a user.
4. [ ] Fill out the appropriate fields for Name, user, etc.
5. [ ] When prompted to assign licenses select as needed Microsoft Entra ID P1 or Microsoft Entra ID P2, then click Next.
6. [ ] Under the Option settings screen you may choose from several types of privileged roles. Choose Admin center access followed by the appropriate role then click Next.
7. [ ] Select Finish adding.

#### Validation and evidence

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Users > Active users.
3. [ ] Sort by the Licenses column.
4. [ ] For each user account in an administrative role verify the account is assigned a license that is not associated with applications i.e. (Microsoft Entra ID P1, Microsoft Entra ID P2). o If an organization uses PIM to elevate a daily driver account to privileged levels, this control and licensing requirement can be considered satisfied.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 1.2.2 Ensure sign-in to shared mailboxes is blocked (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Shared mailboxes are used when multiple people need access to the same mailbox, such as a company information or support email address, reception desk, or other function that might be shared by multiple people.

#### Configuration

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com/
2. [ ] Click to expand Teams & groups and select Shared mailboxes.
3. [ ] Take note of all shared mailboxes.
4. [ ] Click to expand Users and select Active users.
5. [ ] Select a shared mailbox account to open its properties pane and then select Block sign-in.
6. [ ] Check the box for Block this user from signing in.
7. [ ] Repeat for any additional shared mailboxes.

#### Validation and evidence

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com/
2. [ ] Expand Teams & groups and select Shared mailboxes.
3. [ ] Take note of all shared mailboxes.
4. [ ] Expand Users and select Active users.
5. [ ] Select a shared mailbox account to open its properties pane, and review.
6. [ ] Verify that the text under the name reads Sign-in blocked.
7. [ ] Repeat for any additional shared mailboxes.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 1.3.1 Ensure the 'Password expiration policy' is set to 'Set passwords to never expire (recommended)' (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft cloud-only accounts have a pre-defined password policy that cannot be changed.

#### Configuration

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Settings > Org Settings.
3. [ ] Click on Security & privacy.
4. [ ] Check the Set passwords to never expire (recommended) box.
5. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Settings > Org Settings.
3. [ ] Click on Security & privacy.
4. [ ] Select Password expiration policy and verify that Set passwords to never expire (recommended) has been checked.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 1.3.4 Ensure 'User owned apps and services' is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** By default, users can install add-ins in their Microsoft Word, Excel, and PowerPoint applications, allowing data access within the application.

#### Configuration

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Settings > Org settings.
3. [ ] In Services select User owned apps and services.
4. [ ] Uncheck Let users access the Office Store and Let users start trials on behalf of your organization.
5. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Settings > Org settings.
3. [ ] In Services select User owned apps and services.
4. [ ] Verify that Let users access the Office Store and Let users start trials on behalf of your organization are not checked.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 1.3.5 Ensure internal phishing protection for Forms is enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Forms can be used for phishing attacks by asking personal or sensitive information and collecting the results.

#### Configuration

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Settings > Org settings.
3. [ ] Under Services select Microsoft Forms.
4. [ ] Click the checkbox labeled Add internal phishing protection under Phishing protection.
5. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Settings > Org settings.
3. [ ] Under Services select Microsoft Forms.
4. [ ] Verify the checkbox labeled Add internal phishing protection is checked under Phishing protection.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 1.3.9 Ensure shared bookings pages are restricted to select users (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Shared Bookings allows you to invite your team members and create booking pages and let your customers book time with you and your team.

#### Configuration

1. [ ] To remediate using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] Run the following PowerShell command: Set-OwaMailboxPolicy "OwaMailboxPolicy-Default" - BookingsMailboxCreationEnabled $false Optionally: For a more restrictive state Bookings can be disabled at the organization level
4. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
5. [ ] Run the following command: Set-OrganizationConfig -BookingsEnabled $false Note: Disabling Bookings at the tenant (organization) level will be more impactful to end users and is not required for compliance.

#### Validation and evidence

1. [ ] Ensure Shared Bookings is turned off in the OWA Default policy. If booking is disabled at the tenant (OrganizationConfig) level this is also a compliant state. To audit using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] Run the following command: Get-OwaMailboxPolicy -Identity OwaMailboxPolicy-Default | fl BookingsMailboxCreationEnabled
4. [ ] Verify that BookingsMailboxCreationEnabled is set to False. Optionally: If Bookings is disabled at the organization level, this is also considered a compliant state.
5. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
6. [ ] Run the following command: Get-OrganizationConfig | fl BookingsEnabled
7. [ ] If BookingsEnabled is set to False, the organization is using a more restrictive and compliant configuration. In this case changing the default OWA policy would not be required for compliance.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

## 2. Defender and threat protection

### 2.1.2 Ensure the Common Attachment Types Filter is enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The Common Attachment Types Filter is a setting within Exchange Online Protection's anti-malware policy that blocks inbound and outbound email messages containing attachments of specified file types.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules.
3. [ ] On the Policies & rules page select Threat policies.
4. [ ] Under polices select Anti-malware and click on the Default (Default) policy.
5. [ ] On the Policy page that appears on the right hand pane scroll to the bottom and click on Edit protection settings, check the Enable the common attachments filter. o If any of the default file types are missing click Select file types and add the missing file types in. o Reference the Default Value section of this document for the list of extensions that should be blocked.
6. [ ] Click Save to save the changes.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules.
3. [ ] On the Policies & rules page select Threat policies.
4. [ ] Under Policies select Anti-malware and click on the Default (Default) policy.
5. [ ] On the policy page that appears on the righthand pane, under Protection settings, verify that the Enable the common attachments filter has the value of On.
6. [ ] Click on Edit protection settings to view the list of file types that are blocked by the common attachment filter. Verify that the list of file types contains at least the 53 file types found in the Default Value section of this document.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.1.3 Ensure notifications for internal users sending malware is Enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Exchange Online Protection (EOP) is Microsoft's cloud-based filtering service that protects organizations against spam, malware, and other email threats.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand E-mail & Collaboration > Policies & rules.
3. [ ] On the Policies & rules page select Threat policies.
4. [ ] Under Policies select Anti-malware.
5. [ ] Click on the Default (Default) policy.
6. [ ] Click on Edit protection settings and change the settings for Notify an admin about undelivered messages from internal senders to On and enter the email address of the administrator who should be notified under Administrator email address.
7. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand E-mail & Collaboration > Policies & rules.
3. [ ] On the Policies & rules page select Threat policies.
4. [ ] Under Policies select Anti-malware.
5. [ ] Click on the Default (Default) policy.
6. [ ] Verify that Notify an admin about undelivered messages from internal senders is set to On and that there is at least one email address under Administrator email address.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.1.6 Ensure Exchange Online Spam Policies are set to notify administrators (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** In Microsoft 365 organizations with mailboxes in Exchange Online or standalone Exchange Online Protection (EOP) organizations without Exchange Online mailboxes, email messages are automatically protected against spam (junk email) by EOP.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules> Threat policies.
3. [ ] Under Policies select Anti-spam.
4. [ ] Click on the Anti-spam outbound policy (default).
5. [ ] Select Edit protection settings then under Notifications:
6. [ ] Check Send a copy of suspicious outbound messages or message that exceed these limits to these users and groups then enter the desired email addresses.
7. [ ] Check Notify these users and groups if a sender is blocked due to sending outbound spam then enter the desired email addresses.
8. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules > Threat policies.
3. [ ] Under Policies select Anti-spam.
4. [ ] Click on the Anti-spam outbound policy (default).
5. [ ] Verify that Send a copy of suspicious outbound messages or message that exceed these limits to these users and groups is set to On, ensure the email address is correct.
6. [ ] Verify that Notify these users and groups if a sender is blocked due to sending outbound spam is set to On, ensure the email address is correct.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.1.8 Ensure that SPF records are published for all Exchange Domains (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** For each domain that is configured in Exchange, a corresponding Sender Policy Framework (SPF) record should be created.

#### Configuration

1. [ ] To remediate using a DNS provider: For each domain identified as non-compliant during the audit, make the necessary updates in your DNS provider or through your third-party SPF management service. Missing SPF Record: If a domain does not currently have an SPF record, create one similar to the example below, assuming all email is routed through Exchange Online (Microsoft 365 or Microsoft 365 GCC): # Hard fail v=spf1 include:spf.protection.outlook.com -all # Soft fail v=spf1 include:spf.protection.outlook.com ~all Additional Senders: If other authorized email services are used, add their SPF entries using the include: mechanism as needed. For example: v=spf1 include:spf.protection.outlook.com include:exampledomain.net -all

#### Validation and evidence

1. [ ] STEP 1: Determine the list of domains to audit Using the UI:
2. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com
3. [ ] Expand Settings > Domains.
4. [ ] Take note of all custom domains and subdomains defined. o Exclude the (MOERA) domain *.onmicrosoft.com o Exclude the coexistence domain *.mail.onmicrosoft.com (if shown).
5. [ ] Use this list of domains in the audit procedure. Using PowerShell:
6. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
7. [ ] Run the following: Get-AcceptedDomain | Where-Object {$_.IsCoExistenceDomain -eq $false -and $_.InitialDomain -eq $false}
8. [ ] Use this list in the audit procedure. Note: Microsoft owns the tenant's organizational level *.onmicrosoft.com domains, so it is not necessary to create SPF records for the initial (MOERA) or the coexistence (hybrid) domain. STEP 2: Perform the Audit using PowerShell:
9. [ ] Open a PowerShell prompt.
10. [ ] Run the following for each custom domain identified in Step 1 that sends email from Exchange Online: Resolve-DnsName domain1.com -Type TXT | fl Ensure the following criteria are met:
11. [ ] A valid TXT record must begin with v=spf1, which indicates it is SPF v1 (the current standard).
12. [ ] The record must be either directly or indirectly managed: o An indirectly managed record uses a modifier like redirect=[domain], which allows centralized SPF management by a trusted vendor.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.1.9 Ensure that DKIM is enabled for all Exchange Online Domains (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** DKIM is one of the trio of Authentication methods (SPF, DKIM and DMARC) that help prevent attackers from sending messages that look like they come from your domain.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
2. [ ] Expand Email & collaboration > Policies & rules > Threat policies.
3. [ ] Under Rules section click Email authentication settings.
4. [ ] Select DKIM
5. [ ] Select the domain to remediate.
6. [ ] Click Create DKIM keys.
7. [ ] Microsoft provides the properly formatted CNAME records, copy these for later use.
8. [ ] In another browser tab or window, go to the domain registrar for the domain, and then create the two CNAME records using the information from the previous step.
9. [ ] Return the domain properties flyout and toggle Sign messages for this domain with DKIM signatures to Enabled. If successful the status will show Signing DKIM signatures for this domain.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
2. [ ] Expand Email & collaboration > Policies & rules > Threat policies.
3. [ ] Under Rules section click Email authentication settings.
4. [ ] Select DKIM.
5. [ ] For each Accepted domain that is configured to send email: o Skip any *.onmicrosoft.com domain (MOERA or Coexistence), these outbound messages are automatically signed by Microsoft. o Click on the domain name. o Confirm Sign messages for this domain with DKIM signatures is Enabled. o Ensure Status reads Signing DKIM signatures for this domain.
6. [ ] A status of Not signing DKIM signatures for this domain or No DKIM keys saved for this domain is out of compliance.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.1.10 Ensure DMARC records for all Exchange Online domains are published (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** DMARC, or Domain-based Message Authentication, Reporting, and Conformance, assists recipient mail systems in determining the appropriate action to take when messages from a domain fail to meet SPF or DKIM authentication criteria.

#### Configuration

1. [ ] To remediate using a DNS provider:
2. [ ] For any out of compliance domain sending email, add the following record to DNS: Record: _dmarc.domain1.com Type: TXT Value: v=DMARC1; p=none; rua=mailto:<rua-report@example.com>; ruf=mailto:<ruf-report@example.com>
3. [ ] This will create a basic DMARC policy that will allow the organization to start monitoring message statistics.
4. [ ] One week is enough time for data generated by the reports to be useful in understanding email trends and traffic. The final step requires implementing a policy of p=reject OR p=quarantine and pct=100 with the necessary rua and ruf email addresses defined: Record: _dmarc.domain1.com Type: TXT Value: v=DMARC1; p=reject; pct=100; rua=mailto:<rua-report@example.com>; ruf=mailto:<ruf-report@example.com> Parked Domains: For any domain not used for sending email, add the following record to DNS: Record: _dmarc.domain1.com Type: TXT Value: v=DMARC1; p=reject; To remediate the MOERA domain using the UI:
5. [ ] Navigate to the Microsoft 365 admin center https://admin.microsoft.com/
6. [ ] Expand Settings and select Domains.
7. [ ] Select your tenant domain (for example, contoso.onmicrosoft.com).
8. [ ] Select DNS records and click + Add record.
9. [ ] Add a new record with the TXT name of _dmarc with the appropriate values outlined above.

#### Validation and evidence

1. [ ] STEP 1: Determine the list of domains to audit Using the UI:
2. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com
3. [ ] Expand Settings > Domains.
4. [ ] Take note of all custom domains and subdomains defined. o Exclude the coexistence domain *.mail.onmicrosoft.com (if shown).
5. [ ] Include the MOERA domain: [tenant].onmicrosoft.com
6. [ ] Use this list of domains in the audit procedure. Using PowerShell:
7. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
8. [ ] Run the following: Get-AcceptedDomain | Where-Object {$_.IsCoExistenceDomain -eq $false}
9. [ ] Use this list in the audit procedure. STEP 2: Perform the Audit using PowerShell: Note: Resolve-DnsName is not available on versions of Windows earlier than Windows 8 and Windows Server 2012. Use alternatives such as nslookup when needed.
10. [ ] Open a PowerShell prompt.
11. [ ] Run the following for each domain identified in Step 1: Resolve-DnsName _dmarc.domain1.com -Type TXT
12. [ ] Ensure the following criteria are met:

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.1.12 Ensure the connection filter IP allow list is not used (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** In Microsoft 365 organizations with Exchange Online mailboxes or standalone Exchange Online Protection (EOP) organizations without Exchange Online mailboxes, connection filtering and the default connection filter policy identify good or bad source email servers by IP addresses.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules> Threat policies.
3. [ ] Under Policies select Anti-spam.
4. [ ] Click on the Connection filter policy (Default).
5. [ ] Click Edit connection filter policy.
6. [ ] Remove any IP entries from Always allow messages from the following IP addresses or address range:.
7. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules > Threat policies.
3. [ ] Under Policies select Anti-spam.
4. [ ] Click on the Connection filter policy (Default).
5. [ ] Verify that IP Allow list contains no entries.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.1.13 Ensure the connection filter safe list is off (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** In Microsoft 365 organizations with Exchange Online mailboxes or standalone Exchange Online Protection (EOP) organizations without Exchange Online mailboxes, connection filtering and the default connection filter policy identify good or bad source email servers by IP addresses.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules> Threat policies.
3. [ ] Under Policies select Anti-spam.
4. [ ] Click on the Connection filter policy (Default).
5. [ ] Click Edit connection filter policy.
6. [ ] Uncheck Turn on safe list.
7. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules > Threat policies.
3. [ ] Under Policies select Anti-spam.
4. [ ] Click on the Connection filter policy (Default).
5. [ ] Verify that Safe list is Off.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.1.14 Ensure inbound anti-spam policies do not contain allowed domains (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Anti-spam protection is a feature of Exchange Online that utilizes policies to help to reduce the amount of junk email, bulk and phishing emails a mailbox receives.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules> Threat policies.
3. [ ] Under Policies select Anti-spam.
4. [ ] Open each out of compliance inbound anti-spam policy by clicking on it.
5. [ ] Click Edit allowed and blocked senders and domains.
6. [ ] Select Allow domains.
7. [ ] Delete each domain from the domains list.
8. [ ] Click Done > Save.
9. [ ] Repeat as needed.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules > Threat policies.
3. [ ] Under Policies select Anti-spam.
4. [ ] Inspect each inbound anti-spam policy
5. [ ] Verify that Allowed domains does not contain any domain names.
6. [ ] Repeat as needed for any additional inbound anti-spam policy.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.1.15 Ensure outbound anti-spam message limits are in place (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The default outbound anti-spam policy in Microsoft Defender automatically applies to all users and is designed to detect and limit suspicious email-sending behavior.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules> Threat policies.
3. [ ] Under Policies select Anti-spam and click to open Anti-spam outbound policy (Default).
4. [ ] Select Edit protection settings.
5. [ ] Set the following settings to the recommended values, or more restrictive values. Message limit values of 0 are not compliant, as it represents the service default o External: Set an external message limit - 500 o Internal: Set an internal message limit - 1000 o Daily: Set a daily message limit - 1000 o Action: Restriction placed on users who reach the message limit - Restrict the user from sending mail
6. [ ] Verify that Notify these users and groups if a sender is blocked due to sending outbound spam contains a monitored mailbox.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com.
2. [ ] Expand Email & collaboration > Policies & rules > Threat policies.
3. [ ] Under Policies select Anti-spam and click to open Anti-spam outbound policy (Default).
4. [ ] Verify the following settings are configured to the recommended level or a more restrictive value. Message limit values of 0 are not compliant, as it represents the service default: o External: Restrict sending to external recipients (per hour) - 500 o Internal: Restrict sending to internal recipients (per hour) - 1000 o Daily: Maximum recipient limit per day - 1000 o Action: Over limit action - Restrict the user from sending mail
5. [ ] Verify that a monitored mailbox is configured as a recipient under Notify these users and groups if a sender is blocked due to sending outbound spam.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.2.1 Ensure emergency access account activity is monitored (Manual)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Organizations should monitor sign-in and audit log activity from the emergency accounts and trigger notifications to other administrators.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com
2. [ ] Under the Cloud Apps section select Policies -> Policy management.
3. [ ] Click on All policies and then Create policy -> Activity policy.
4. [ ] Give the policy a name and set the following: o Policy severity to High severity. o Category to Privileged accounts. o Act on Single activity. o Click Select a filter -> Activity type equals Log on. o Click Add a filter -> User Name equals <Emergency access account> as Any role. o Ensure all emergency access accounts are added to this policy or another. o Select an alert method such as Send alert as email.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com
2. [ ] Under the Cloud Apps section select Policies -> Policy management.
3. [ ] Locate a privileged accounts policy that meets the following criteria o Policy severity is High severity. o Category is Privileged accounts. o Act on Single activity is selected. o Under Activities matching all of the following verify: o Filter1: Activity type equals Log on o Filter2: User Name equals <Emergency access account> as Any role o Verify all additional emergency access accounts are accounted for. o Under Alerts, verify alerting is configured.
4. [ ] Repeat this process for any additional emergency access or break-glass accounts in the organization. If matching policies do not exist, then the audit procedure is considered a fail.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.4.1 Ensure Priority account protection is enabled and configured (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Identify priority accounts to utilize Microsoft 365's advanced custom security features.

#### Configuration

1. [ ] Remediate with a 3-step process Step 1: Enable Priority account protection in Microsoft 365 Defender:
2. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
3. [ ] Select System > Settings near the bottom of the left most panel.
4. [ ] Select E-mail & Collaboration > Priority account protection
5. [ ] Ensure Priority account protection is set to On Step 2: Tag priority accounts:
6. [ ] Select User tags
7. [ ] Select the PRIORITY ACCOUNT tag and click Edit
8. [ ] Select Add members to add users, or groups. Groups are recommended.
9. [ ] Repeat the previous 2 steps for any additional tags needed, such as Finance or HR.
10. [ ] Next and Submit. Step 3: Configure E-mail alerts for Priority Accounts:
11. [ ] Expand E-mail & Collaboration on the left column.
12. [ ] Select Policies & rules > Alert policy

#### Validation and evidence

1. [ ] Audit with a 3-step process Step 1: Verify Priority account protection is enabled:
2. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
3. [ ] Select System > Settings near the bottom of the left most panel.
4. [ ] Select E-mail & collaboration > Priority account protection
5. [ ] Verify that Priority account protection is set to On Step 2: Verify that priority accounts are identified and tagged accordingly:
6. [ ] Select User tags
7. [ ] Select the PRIORITY ACCOUNT tag and click Edit
8. [ ] Verify the assigned members match the organization's defined priority accounts or groups.
9. [ ] Repeat the previous 2 steps for any additional tags identified, such as Finance or HR. Step 3: Ensure alerts are configured:
10. [ ] Expand E-mail & Collaboration on the left column.
11. [ ] Select Policies & rules > Alert policy
12. [ ] Verify that at least two alert policies are configured to monitor priority accounts for the activities Detected malware in an email message and Phishing email detected at time of delivery. These alerts should meet the following criteria: o Severity: High o Category: Threat management o Mail Direction: Inbound o Recipient Tags: Includes Priority account

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.4.2 Ensure Priority accounts have 'Strict protection' presets applied (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Preset security policies have been established by Microsoft, utilizing observations and experiences within datacenters to strike a balance between the exclusion of malicious content from users and limiting unwarranted disruptions.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
2. [ ] Expand E-mail & collaboration > Policies & rules > Threat policies.
3. [ ] Select Preset security policies.
4. [ ] Click to Manage protection settings for Strict protection preset.
5. [ ] For Apply Exchange Online Protection select at minimum Specific recipients and include the Accounts/Groups identified as Priority Accounts.
6. [ ] For Apply Defender for Office 365 Protection select at minimum Specific recipients and include the Accounts/Groups identified as Priority Accounts.
7. [ ] For Impersonation protection click Next and add valid e-mails or priority accounts both internal and external that may be subject to impersonation.
8. [ ] For Protected custom domains add the organization's domain name, along side other key partners.
9. [ ] Click Next and finally Confirm

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
2. [ ] Expand E-mail & collaboration > Policies & rules > Threat policies.
3. [ ] From here visit each section in turn: Anti-phishing Anti-spam Anti-malware Safe Attachments Safe Links
4. [ ] Verify that each contains a policy named Strict Preset Security Policy that includes the organization's priority accounts and groups.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.4.4 Ensure Zero-hour auto purge for Microsoft Teams is on (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Zero-hour auto purge (ZAP) is a protection feature that retroactively detects and neutralizes malware and high confidence phishing.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
2. [ ] Expand System > Settings > Email & collaboration > Microsoft Teams protection.
3. [ ] Set Zero-hour auto purge (ZAP) to On (Default)

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
2. [ ] Expand System > Settings > Email & collaboration > Microsoft Teams protection.
3. [ ] Verify that Zero-hour auto purge (ZAP) is set to On (Default)
4. [ ] Under Exclude these participants review the list of exclusions and verify they are justified and within tolerance for the organization.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 2.4.5 Ensure 'AIR' remediation is enabled (Manual)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Automated Investigation and Response (AIR) investigates alerts and correlates related signals into investigations.

#### Configuration

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
2. [ ] Expand System > Settings > Email & collaboration > MDO automation settings.
3. [ ] Under Message clusters check the following: o Similar files o Similar URLs o Multiple similar attributes
4. [ ] Click Save to apply the changes.

#### Validation and evidence

1. [ ] Navigate to Microsoft Defender https://security.microsoft.com/
2. [ ] Expand System > Settings > Email & collaboration > MDO automation settings.
3. [ ] Verify that under Message clusters the following are checked: o Similar files o Similar URLs o Multiple similar attributes

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

## 3. Purview and information protection

### 3.1.1 Ensure Microsoft 365 audit log search is Enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** When audit log search is enabled in the Microsoft Purview compliance portal, user and admin activity within the organization is recorded in the audit log and retained for 180 days by default.

#### Configuration

1. [ ] Navigate to Microsoft Purview https://purview.microsoft.com/
2. [ ] Select Solutions and then Audit to open the audit search.
3. [ ] Click blue bar Start recording user and admin activity.
4. [ ] Click Yes on the dialog box to confirm.

#### Validation and evidence

1. [ ] Navigate to Microsoft Purview https://purview.microsoft.com/
2. [ ] Select Solutions and then Audit to open the audit search.
3. [ ] Choose a date and time frame in the past 30 days.
4. [ ] Verify search capabilities (e.g. try searching for Activities as Accessed file and results should be displayed).

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 3.2.1 Ensure DLP policies are enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Data Loss Prevention (DLP) policies allow Exchange Online and SharePoint Online content to be scanned for specific types of data like social security numbers, credit card numbers, or passwords.

#### Configuration

1. [ ] Navigate to Microsoft Purview https://purview.microsoft.com/
2. [ ] Click Solutions > Data loss prevention then Policies.
3. [ ] Click Create policy.
4. [ ] Create a policy that is specific to the types of data the organization wishes to protect.

#### Validation and evidence

1. [ ] Navigate to Microsoft Purview https://purview.microsoft.com/
2. [ ] Click Solutions > Data loss prevention and then Policies.
3. [ ] Inspect the list of policies and verify the following criteria: o A policy exists that meets the organizations DLP needs o Mode is On
4. [ ] Open the policy and verify there is at least one of the following locations defined: o Exchange email o SharePoint sites o OneDrive accounts o Teams chat and channel messages
5. [ ] Compliance is met when there is at least one policy the meets the above criteria.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 3.2.2 Ensure DLP policies are enabled for Microsoft Teams (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The default Teams Data Loss Prevention (DLP) policy rule in Microsoft 365 is a preconfigured rule that is automatically applied to all Teams conversations and channels.

#### Configuration

1. [ ] Navigate to Microsoft Purview compliance portal https://purview.microsoft.com/
2. [ ] Under Solutions select Data loss prevention then Policies.
3. [ ] Click Policies tab.
4. [ ] Check Default policy for Teams then click Edit policy.
5. [ ] The edit policy window will appear click Next
6. [ ] At the Choose locations to apply the policy page, turn the status toggle to On for Teams chat and channel messages location and then click Next.
7. [ ] On Customized advanced DLP rules page, ensure the Default Teams DLP policy rule Status is On and click Next.
8. [ ] On the Policy mode page, select the radial for Turn it on right away and click Next.
9. [ ] Review all the settings for the created policy on the Review your policy and create it page, and then click submit.
10. [ ] Once the policy has been successfully submitted click Done.

#### Validation and evidence

1. [ ] Navigate to Microsoft Purview compliance portal https://purview.microsoft.com/
2. [ ] Under Solutions select Data loss prevention then Policies.
3. [ ] Locate the Default policy for Teams.
4. [ ] Verify the Status is On.
5. [ ] Verify Locations include Teams chat and channel messages - All accounts.
6. [ ] Verify Policy settings includes the Default Teams DLP policy rule or one specific to the organization.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 3.2.3 Ensure DLP policies are published for Copilot users (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Purview Data Loss Prevention (DLP) policies can be scoped to Microsoft 365 Copilot and Copilot Chat interactions.

#### Configuration

1. [ ] Note: Microsoft provides a guided wizard to create the Default DLP policy - Protect sensitive M365 Copilot interactions policy, which can be used when no Copilot DLP policy exists in the tenant. The steps below describe how to create a custom policy from scratch with Copilot included as a location.
2. [ ] Navigate to Microsoft Purview compliance portal https://purview.microsoft.com/
3. [ ] Under Solutions select Data loss prevention then Policies.
4. [ ] Click Policies tab.
5. [ ] Click + Create Policy.
6. [ ] Click on Enterprise applications & devices.
7. [ ] Under Categories select Custom and then Custom policy for the regulation.
8. [ ] Name the policy, and if appropriate, select an Admin Unit.
9. [ ] In Locations select Microsoft 365 Copilot and Copilot Chat.
10. [ ] Click on Next to proceed to the Advanced DLP rules page.
11. [ ] Click on + Create Rule
12. [ ] Name the rule and give a brief description of the data that is being targeted.

#### Validation and evidence

1. [ ] Navigate to Microsoft Purview compliance portal https://purview.microsoft.com/
2. [ ] Under Solutions select Data loss prevention then Policies.
3. [ ] Inspect the list of policies and verify the following criteria: o Locations includes Microsoft 365 Copilot and Copilot Chat - All accounts. o Mode is On. o The policy includes Rules that restrict sensitive data from being shared in Copilot interactions based on the organization's needs.
4. [ ] Compliance is met when there is at least one policy that meets the above criteria.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 3.3.1 Ensure Information Protection sensitivity label policies are published (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Sensitivity labels enable organizations to classify and label content across Microsoft 365 based on its sensitivity and business impact.

#### Configuration

1. [ ] Navigate to Microsoft Purview compliance portal https://purview.microsoft.com/
2. [ ] Select Information protection > Sensitivity labels.
3. [ ] Click Create a label to create a label.
4. [ ] Click Publish labels and select any newly created labels to publish according to the organization's information protection needs.

#### Validation and evidence

1. [ ] Navigate to Microsoft Purview compliance portal https://purview.microsoft.com/
2. [ ] Select Information protection > Policies > Label publishing policies.
3. [ ] Ensure that a Label policy exists and is published according to the organization's information protection needs.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

## 4. Intune and endpoint management

### 4.1 Ensure devices without a compliance policy are marked 'not compliant' (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Compliance policies are sets of rules and conditions that are used to evaluate the configuration of managed devices.

#### Configuration

1. [ ] Navigate to Microsoft Intune admin center https://intune.microsoft.com/
2. [ ] Select Devices and then under Manage devices click Compliance
3. [ ] Click Compliance settings.
4. [ ] Set Mark devices with no compliance policy assigned as to Not compliant.

#### Validation and evidence

1. [ ] Navigate to Microsoft Intune admin center https://intune.microsoft.com/
2. [ ] Select Devices and then under Manage devices click Compliance
3. [ ] Click Compliance settings.
4. [ ] Verify that Mark devices with no compliance policy assigned as is set to Not compliant.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 4.2 Ensure device enrollment for personally owned devices is blocked by default (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Device enrollment restrictions let you restrict devices from enrolling in Intune based on certain device attributes such as device limit, device platform, OS Version, manufacturer or device ownership (Personally owned devices).

#### Configuration

1. [ ] Navigate to Microsoft Intune admin center https://intune.microsoft.com/
2. [ ] Select Devices and then under Device onboarding click Enrollment
3. [ ] Under Enrollment options select Device platform restriction.
4. [ ] Inspect the policies listed under Device type restrictions o For the Default priority policy, click All Users. o Select Properties.
5. [ ] Click Edit to change Platform settings.
6. [ ] In the Personally owned column set each platform to Block.

#### Validation and evidence

1. [ ] Navigate to Microsoft Intune admin center https://intune.microsoft.com/
2. [ ] Select Devices and then under Device onboarding click Enrollment
3. [ ] Under Enrollment options select Device platform restriction.
4. [ ] Inspect the policies listed under Device type restrictions o For the Default priority policy, click All Users. o Select Properties.
5. [ ] Verify that all platforms are set to Block in the Personally owned column.
6. [ ] If the Platform itself is set to Block for any of the platforms shown this is also a passing state for that platform.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

## 5. Entra ID and Conditional Access

### 5.1.2.1 Ensure 'Per-user MFA' is disabled (Manual)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Legacy per-user Multi-Factor Authentication (MFA) can be configured to require individual users to provide multiple authentication factors, such as passwords and additional verification codes, to access their accounts.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Users and select All users.
3. [ ] Click on Per-user MFA on the top row.
4. [ ] Click the empty box next to Display Name to select all accounts.
5. [ ] On the far right under quick steps click Disable.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Users and select All users.
3. [ ] Click on Per-user MFA on the top row.
4. [ ] Verify that the Multi-factor Auth Status column shows Disabled for each account.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.2.2 Ensure users cannot register applications (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting controls whether standard users can register applications in the Microsoft Entra ID directory.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Users and select Users settings.
3. [ ] Set Users can register applications to No.
4. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Users and select Users settings.
3. [ ] Verify that Users can register applications is set to No.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.2.3 Ensure 'Restrict non-admin users from creating tenants' is set to 'Yes' (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Non-privileged users can create tenants in the Microsoft Entra ID and Microsoft Entra administration portal under "Manage tenant".

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand Entra ID > Users and select User settings.
3. [ ] Set Restrict non-admin users from creating tenants to Yes then Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand Entra ID > Users and select User settings.
3. [ ] Verify that Restrict non-admin users from creating tenants is set to Yes

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.2.4 Ensure access to the Entra admin center is restricted (Manual)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting restricts non-administrators from loading a set of frequently visited pages in the Microsoft Entra admin center and Azure portal, including home, tenant overview, and the users list.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand Entra ID > Users and select User settings.
3. [ ] Set Restrict access to Microsoft Entra admin center to Yes then Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand Entra ID > Users and select User settings.
3. [ ] Verify under the Administration center section that Restrict access to Microsoft Entra admin center is set to Yes.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.3.1 Ensure users cannot create security groups (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting allows users in the organization to create new security groups and add members to these groups in the Azure portal, API, or PowerShell.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Groups and select General.
3. [ ] Set Users can create security groups in Azure portals, API or

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Groups and select General.
3. [ ] Verify that Users can create security groups in Azure portals, API or PowerShell is set to No.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.3.3 Ensure that 'Owners can manage group membership requests in My Groups' is set to 'No' (Manual)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Entra ID provides self-service group management features that enable users to create and manage their own security groups or Microsoft 365 groups.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Groups select General.
3. [ ] Set Owners can manage group membership requests in My Groups to No.
4. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Groups and select General.
3. [ ] Verify that Owners can manage group membership requests in My Groups is set to No

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.4.2 Ensure the maximum number of devices per user is limited (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting defines the maximum number of Microsoft Entra joined or registered devices that a user can have in Microsoft Entra ID.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Devices and select Device settings.
3. [ ] Set Maximum number of devices per user to 10 or less.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Devices and select Device settings.
3. [ ] Verify that Maximum number of devices per user is set to 10 or less.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.4.3 Ensure the GA role is not added as a local administrator during Entra join (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting controls whether the Global Administrator role is automatically added to the local administrators group on a device during the Microsoft Entra join process.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Devices and select Device settings.
3. [ ] Set Global administrator role is added as local administrator on the device during Microsoft Entra join (Preview) to No.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Devices and select Device settings.
3. [ ] Verify that Global administrator role is added as local administrator on the device during Microsoft Entra join (Preview) is set to No.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.4.4 Ensure local administrator assignment is limited during Entra join (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting determines if the Microsoft Entra user registering their device as Microsoft Entra join will be added to the local administrators group.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Devices and select Device settings.
3. [ ] Set Registering user is added as local administrator on the device during Microsoft Entra join (Preview) to Selected (and add members) or None.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Devices and select Device settings.
3. [ ] Verify that Registering user is added as local administrator on the device during Microsoft Entra join (Preview) is set to Selected or None.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.4.5 Ensure Local Administrator Password Solution is enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Local Administrator Password Solution (LAPS) is the management of local account passwords on Windows devices.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Devices and select Device settings.
3. [ ] Set Enable Microsoft Entra Local Administrator Password Solution (LAPS) to Yes.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Devices and select Device settings.
3. [ ] Verify that Enable Microsoft Entra Local Administrator Password Solution (LAPS) is set to Yes.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.5.2 Ensure the admin consent workflow is enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The admin consent workflow gives admins a secure way to grant access to applications that require admin approval.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID and select Enterprise apps.
3. [ ] Under Security select Consent and permissions.
4. [ ] Under Manage select Admin consent settings.
5. [ ] Set Users can request admin consent to apps they are unable to consent to to Yes under Admin consent requests.
6. [ ] Under the Reviewers choose the Roles and Groups that will review user generated app consent requests.
7. [ ] Set Selected users will receive email notifications for requests to Yes
8. [ ] Select Save at the top of the window.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID and select Enterprise apps.
3. [ ] Under Security select Consent and permissions.
4. [ ] Under Manage select Admin consent settings.
5. [ ] Verify that Users can request admin consent to apps they are unable to consent to is set to Yes.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.5.4 Ensure password lifetime for applications does not exceed 180 days (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** In Microsoft Entra ID, applications and service principals can authenticate using password credentials (also referred to as client secrets).

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID and select Enterprise apps.
3. [ ] Under Security select Application policies.
4. [ ] Select Restrict max password lifetime.
5. [ ] Set Status to On.
6. [ ] Set the maximum lifetime to 180 days or less.
7. [ ] Set Applies to to one of the following: o All applications o All applications with exclusions (if using exclusions, ensure they are reviewed annually).
8. [ ] Set Only apply to apps created after to a desired date or leave it unconfigured.
9. [ ] Select Save and close to apply the changes.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID and select Enterprise apps.
3. [ ] Under Security select Application policies.
4. [ ] Select Restrict max password lifetime.
5. [ ] Verify that Status is set to On.
6. [ ] Verify that the configured maximum lifetime is 180 days or less.
7. [ ] Verify that Applies to is set to one of the following: o All applications o All applications with exclusions (if using exclusions, verify they are reviewed annually).
8. [ ] Verify that Only apply to apps created after is one of the following states: o Not configured (Field will show Select a date with no date selected) o A date that is on or before the date of the assessment.
9. [ ] Compliance is met when all of the above conditions are satisfied.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.5.5 Ensure new application passwords are system-generated (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** In Microsoft Entra ID, applications and service principals can authenticate using password credentials (also referred to as client secrets).

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID and select Enterprise apps.
3. [ ] Under Security select Application policies.
4. [ ] Select Block custom passwords.
5. [ ] Set Status to On.
6. [ ] Set Applies to to one of the following: o All applications o All applications with exclusions (if using exclusions, ensure they are reviewed annually).
7. [ ] Set Only apply to apps created after to a desired date or leave it unconfigured.
8. [ ] Select Save and close to apply the changes.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID and select Enterprise apps.
3. [ ] Under Security select Application policies.
4. [ ] Select Block custom passwords.
5. [ ] Verify that Status is set to On.
6. [ ] Verify that Applies to is set to one of the following: o All applications o All applications with exclusions (if using exclusions, verify they are reviewed annually).
7. [ ] Verify that Only apply to apps created after is one of the following states: o Not configured (Field will show Select a date with no date selected) o A date that is on or before the date of the assessment.
8. [ ] Compliance is met when all of the above conditions are satisfied.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.5.6 Ensure maximum certificate lifetime for applications does not exceed 180 days (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** In Microsoft Entra ID, applications and service principals can authenticate using certificate credentials.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID and select Enterprise apps.
3. [ ] Under Security select Application policies.
4. [ ] Select Restrict max certificate lifetime.
5. [ ] Set Status to On.
6. [ ] Set Applies to to one of the following: o All applications o All applications with exclusions (if using exclusions, ensure they are reviewed annually).
7. [ ] Set Only apply to apps created after to a desired date or leave it unconfigured.
8. [ ] Set Maximum lifetime (in days) to 180 days or less.
9. [ ] Select Save and close to apply the changes.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID and select Enterprise apps.
3. [ ] Under Security select Application policies.
4. [ ] Select Restrict max certificate lifetime.
5. [ ] Verify that Status is set to On.
6. [ ] Verify that Applies to is set to one of the following: o All applications o All applications with exclusions (if using exclusions, verify they are reviewed annually).
7. [ ] Verify that Only apply to apps created after is one of the following states: o Not configured (Field will show Select a date with no date selected) o A date that is on or before the date of the assessment.
8. [ ] Verify that Maximum lifetime (in days) is 180 days or less.
9. [ ] Compliance is met when all of the above conditions are satisfied.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.6.2 Ensure that guest user access is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Entra ID, part of Microsoft Entra, allows you to restrict what external guest users can see in their organization in Microsoft Entra ID.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > External Identities and select External collaboration settings.
3. [ ] Under Guest user access set Guest user access restrictions to one of the following: o Guest users have limited access to properties and memberships of directory objects o Guest user access is restricted to properties and memberships of their own directory objects (most restrictive)

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > External Identities and select External collaboration settings.
3. [ ] Under Guest user access verify that Guest user access restrictions is set to one of the following: o Guest users have limited access to properties and memberships of directory objects o Guest user access is restricted to properties and memberships of their own directory objects (most restrictive)

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.1.8.1 Ensure that password hash sync is enabled for hybrid deployments (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Password Hash Synchronization is one of the sign-in methods used to enable hybrid identity authentication.

#### Configuration

1. [ ] To remediate using the on-prem Microsoft Entra Connect tool:
2. [ ] Log in to the on premises server that hosts the Microsoft Entra Connect tool
3. [ ] Double-click the Azure AD Connect icon that was created on the desktop
4. [ ] Click Configure.
5. [ ] On the Additional tasks page, select Customize synchronization options and click Next.
6. [ ] Enter the username and password for your global administrator.
7. [ ] On the Connect your directories screen, click Next.
8. [ ] On the Domain and OU filtering screen, click Next.
9. [ ] On the Optional features screen, check Password hash synchronization and click Next.
10. [ ] On the Ready to configure screen click Configure.
11. [ ] Once the configuration completes, click Exit.

#### Validation and evidence

1. [ ] Only Global Admin and Hybrid Identity Administrator roles have access to view the actual Password Hash Sync status message. Inadequate role access will result in a default message stating: "Unable to retrieve your tenant’s password hash sync information."
2. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
3. [ ] Expand Entra ID > Entra Connect.
4. [ ] Select Connect Sync.
5. [ ] Under Microsoft Entra Connect sync, verify the Password Hash Sync status message indicates that synchronization is occurring and no errors are present, with one of the following messages: o Password hash synchronization is enabled o Password hash synchronization cloud configuration is enabled o Password hash synchronization heartbeat detected

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.1 Ensure multifactor authentication is enabled for all users in administrative roles (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Multifactor authentication is a process that requires an additional form of identification during the sign-in process, such as a code from a mobile device or a fingerprint scan, to enhance security.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Click New policy. o Under Users or agents (Preview) include Select users and groups and check Directory roles. o At a minimum, include the directory roles listed below in this section of the document. o Under Target resources include All resources (formerly 'All cloud apps') and do not create any exclusions. ▪ Under Exclude exclude any break-glass accounts. o Under Grant select Grant Access and check either Require multifactor authentication or Require authentication strength. o Click Select at the bottom of the pane.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On. At minimum these directory roles should be included for MFA:
7. [ ] Application administrator
8. [ ] Authentication administrator
9. [ ] Billing administrator
10. [ ] Cloud application administrator
11. [ ] Conditional Access administrator
12. [ ] Exchange administrator

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify Directory roles specific to administrators are included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify All resources (formerly 'All cloud apps') is selected with no exclusions. o Under Grant verify Grant Access is on and either Require multifactor authentication or Require authentication strength is checked.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.2 Ensure multifactor authentication is enabled for all users (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Enable multifactor authentication for all users in the Microsoft 365 tenant.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Click New policy. o Under Users or agents (Preview) include All users. o Under Target resources include All resources (formerly 'All cloud apps') and do not create any exclusions. ▪ Under Exclude exclude any break-glass accounts. o Under Grant select Grant Access and check either Require multifactor authentication or Require authentication strength. o Click Select at the bottom of the pane.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify All users is included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify All resources (formerly 'All cloud apps') is selected with no exclusions. o Under Grant verify Grant Access and either Require multifactor authentication or Require authentication strength is checked.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.3 Enable Conditional Access policies to block legacy authentication (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Entra ID supports the most widely used authentication and authorization protocols including legacy authentication.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Create a new policy by selecting New policy. o Under Users or agents (Preview) include All users. o Under Target resources include All resources (formerly 'All cloud apps'). ▪ Under Exclude exclude any break-glass accounts. o Under Conditions select Client apps and check the boxes for Exchange ActiveSync clients and Other clients. o Under Grant select Block Access. o Click Select.
4. [ ] Set the policy On and click Create.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify All users is included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify All resources (formerly 'All cloud apps') is selected. o Verify that only documented resource exclusions exist and that they are reviewed annually. o Under Conditions select Client apps then verify Exchange ActiveSync clients and Other clients is checked. o Under Grant verify Block access is selected.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.4 Ensure Sign-in frequency is enabled and browser sessions are not persistent for Administrative users (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** In complex deployments, organizations might have a need to restrict authentication sessions.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Click New policy. o Under Users or agents (Preview) include Select users and groups and check Directory roles. o At a minimum, include the directory roles listed below in this section of the document. o Under Target resources include All resources (formerly 'All cloud apps'). ▪ Under Exclude exclude any break-glass accounts. o Under Grant select Grant Access and check Require multifactor authentication. o Under Session select Sign-in frequency select Periodic reauthentication and set it to 4 hours (or less). o Check Persistent browser session then select Never persistent in the drop-down menu.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On. At minimum these directory roles should be included in the policy:
7. [ ] Application administrator
8. [ ] Authentication administrator
9. [ ] Billing administrator
10. [ ] Cloud application administrator
11. [ ] Conditional Access administrator
12. [ ] Exchange administrator

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify Directory roles specific to administrators are included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify All resources (formerly 'All cloud apps') is selected. o Verify that only documented resource exclusions exist and that they are reviewed annually. o Under Session verify Sign-in frequency is checked and set to Periodic reauthentication. o Verify the timeframe is set to the time determined by the organization. o Verify that Periodic reauthentication does not exceed 4 hours (or less). o Verify that Persistent browser session is set to Never persistent.
4. [ ] Verify that Enable policy is set to On

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.6 Enable Identity Protection user risk policies (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Entra ID Protection user risk policies detect the probability that a user account has been compromised.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Create a new policy by selecting New policy. o Under Users or agents (Preview) choose All users o Under Target resources choose All resources (formerly 'All cloud apps') ▪ Under Exclude exclude any break-glass accounts. o Under Conditions choose User risk then Yes and select the user risk level High. o Under Grant select Grant access then check Require multifactor authentication or Require authentication strength. Finally check Require password change. o Under Session set Sign-in frequency to Every time. o Click Select.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify All users is included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify All resources (formerly 'All cloud apps') is selected. o Under Conditions verify User risk is set to High. o Under Grant verify Grant access is selected and either Require multifactor authentication or Require authentication strength are checked. Then verify Require password change is checked. o Under Session ensure Sign-in frequency is set to Every time.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.7 Enable Identity Protection sign-in risk policies (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Entra ID Protection sign-in risk detects risks in real-time and offline.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Create a new policy by selecting New policy. o Under Users or agents (Preview) choose All users. o Under Target resources choose All resources (formerly 'All cloud apps'). ▪ Under Exclude exclude any break-glass accounts. o Under Conditions choose Sign-in risk then Yes and check the risk level boxes High and Medium. o Under Grant click Grant access then select Require multifactor authentication. o Under Session select Sign-in Frequency and set to Every time. o Click Select.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify All users is included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify All resources (formerly 'All cloud apps') is selected. o Under Conditions verify Sign-in risk is set to Yes ensuring High and Medium are selected. o Under Grant verify grant Grant access is selected and Require multifactor authentication checked. o Under Session verify Sign-in Frequency is set to Every time.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.9 Ensure a managed device is required for authentication (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Conditional Access (CA) can be configured to enforce access based on the device's compliance status or whether it is Entra hybrid joined.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Create a new policy by selecting New policy. o Under Users or agents (Preview) include All users. o Under Target resources include All resources (formerly 'All cloud apps'). ▪ Under Exclude exclude any break-glass accounts. o Under Grant select Grant access. o Select the checkbox Require device to be marked as compliant. o Optionally, also select Require Microsoft Entra hybrid joined device if the organization uses hybrid joined devices. o Choose Require one of the selected controls. o Click Select at the bottom.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify All users is included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify All resources (formerly 'All cloud apps') is selected. o Verify that only documented resource exclusions exist and that they are reviewed annually. o Under Grant verify that Require device to be marked as compliant is checked. o Under Grant verify that no other controls are checked except, optionally, Require Microsoft Entra hybrid joined device. o Verify Require one of the selected controls is selected.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.10 Ensure a managed device is required to register security information (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Conditional Access (CA) can be configured to enforce access based on the device's compliance status or whether it is Entra hybrid joined.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Create a new policy by selecting New policy. o Under Users or agents (Preview) include All users. o Under Target resources select User actions and check Register security information. ▪ Under Exclude exclude any break-glass accounts. o Under Grant select Grant access. o Select the checkbox Require device to be marked as compliant. o Optionally, also select Require Microsoft Entra hybrid joined device if the organization uses hybrid joined devices. o Choose Require one of the selected controls. o Click Select at the bottom.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify All users is included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify User actions is selected with Register security information checked. o Under Grant verify that Require device to be marked as compliant is checked. o Under Grant verify that no other controls are checked except, optionally, Require Microsoft Entra hybrid joined device. o Verify Require one of the selected controls is selected.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.11 Ensure sign-in frequency for Intune Enrollment is set to 'Every time' (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Sign-in frequency defines the time period before a user is asked to sign in again when attempting to access a resource.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Create a new policy by selecting New policy. o Under Users or agents (Preview) include All users. o Under Target resources select Resources (formerly cloud apps), choose Select resources and add Microsoft Intune Enrollment to the list. ▪ Under Exclude exclude any break-glass accounts. o Under Grant select Grant access. o Check either Require multifactor authentication or Require authentication strength. o Under Session check Sign-in frequency and select Every time.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify All users is included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify Resources (formerly cloud apps) includes Microsoft Intune Enrollment. o Under Grant verify Require multifactor authentication or Require authentication strength is checked. o Under Session verify Sign-in frequency is set to Every time.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.12 Ensure the device code sign-in flow is blocked (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The Microsoft identity platform supports the device authorization grant, which allows users to sign in to input-constrained devices such as a smart TV, IoT device, or a printer.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Create a new policy by selecting New policy. o Under Users or agents (Preview) include All users. o Under Target resources > Resources (formerly cloud apps) include All resources (formerly 'All cloud apps'). ▪ Under Exclude exclude any break-glass accounts. o Under Conditions > Authentication flows set Configure to Yes and check Device code flow. o Click Save. o Under Grant select Block access and click Select.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to `On

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify All users is included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify Resources (formerly cloud apps) includes All resources (formerly 'All cloud apps') o Under Conditions > Authentication flows verify Configure is set to Yes and Device code flow is checked. o Under Grant verify Block access is selected.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.13 Ensure that periodic reauthentication is required for all users (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Sign-in frequency defines the time period before a user is asked to sign in again when attempting to access a resource.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Create a new policy by selecting New policy. o Under Users or agents (Preview) include All users. o Under Target resources verify Resources (formerly cloud apps) include All resources (formerly 'All cloud apps'). ▪ Under Exclude exclude any break-glass accounts. o Under Session select Sign-in frequency and set Periodic reauthentication to 7 days or less.
4. [ ] Under Enable policy set it to Report-only.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access and select Policies.
3. [ ] Verify that a policy exists with the following criteria and is set to On: o Under Users or agents (Preview) verify All users is included. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify Resources (formerly cloud apps) includes All resources (formerly 'All cloud apps') o Under Session ensure Sign-in frequency is checked, and Periodic reauthentication is set to 7 days or less.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.2.17 Ensure authentication transfer is blocked (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Authentication transfer is a flow that lets users seamlessly transfer authenticated state from one device to another.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access.
3. [ ] Create a new policy by selecting New policy. o Under Users or agents (Preview) include All users. o Under Target resources > Resources (formerly cloud apps) include All resources (formerly 'All cloud apps'). ▪ Under Exclude exclude any break-glass accounts. o Under Conditions > Authentication flows set Configure to Yes and check Authentication transfer. ▪ Click Save. o Under Grant select Block access and click Select.
4. [ ] Under Enable policy set it to Report-only until the organization is ready to enable it.
5. [ ] Click Create.
6. [ ] After allowing the policy to run in Report-only mode for at least one week, review the Sign-in logs for any unexpected impact, then return to the policy and set Enable policy to On.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Conditional Access.
3. [ ] Verify that a policy exists with the following criteria: o Under Users or agents (Preview) verify All users is selected. o Verify that only documented user exclusions exist and that they are reviewed annually. o Under Target resources verify Resources (formerly cloud apps) includes All resources (formerly 'All cloud apps') o Under Conditions > Authentication flows verify Configure is set to Yes and Authentication transfer is checked. o Under Grant verify Block access is selected.
4. [ ] Verify that Enable policy is set to On.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.3.1 Ensure Microsoft Authenticator is configured to protect against MFA fatigue (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft provides supporting settings to enhance the configuration of the Microsoft Authenticator application.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Click to expand Entra ID > Authentication methods and select Policies.
3. [ ] Select Microsoft Authenticator
4. [ ] Under Enable and Target ensure the setting is set to Enable.
5. [ ] Select Configure
6. [ ] Set the following Microsoft Authenticator settings: o Show application name in push and passwordless notifications Status is set to Enabled, Target All users o Show geographic location in push and passwordless notifications Status is set to Enabled, Target All users

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Authentication methods and select Policies.
3. [ ] Under Method select Microsoft Authenticator.
4. [ ] Under Enable and Target verify the setting is set to Enable.
5. [ ] In the Include tab verify that All users is selected.
6. [ ] In the Exclude tab verify only valid groups are present (i.e. Break Glass accounts).
7. [ ] Select Configure
8. [ ] Verify the following Microsoft Authenticator settings: o Show application name in push and passwordless notifications Status is set to Enabled, Target All users o Show geographic location in push and passwordless notifications Status is set to Enabled, Target All users
9. [ ] In each setting select Exclude and verify only valid groups are present (i.e. Break Glass accounts).

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.3.2 Ensure custom banned passwords lists are used (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** With Entra Password Protection, default global banned password lists are automatically applied to all users in an Entra ID tenant.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand Entra ID > Authentication methods and select Password protection.
3. [ ] Set Enforce custom list to Yes
4. [ ] In Custom banned password list create a list using suggestions outlined in this document.
5. [ ] Click Save

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand Entra ID > Authentication methods and select Password protection.
3. [ ] Verify that Enforce custom list is set to Yes
4. [ ] Verify that Custom banned password list contains entries specific to the organization or matches a pre-determined list.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.3.3 Ensure password protection is enabled for on-prem Active Directory (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Entra Password Protection provides a global and custom banned password list.

#### Configuration

1. [ ] Download and install the Azure AD Password Proxies and DC Agents from the following location: https://www.microsoft.com/download/details.aspx?id=57071 After installed follow the steps below.
2. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
3. [ ] Expand Entra ID > Authentication methods and select Password protection.
4. [ ] Set Enable password protection on Windows Server Active Directory to Yes and Mode to Enforced.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select Password protection.
3. [ ] Verify that Enable password protection on Windows Server Active Directory is set to Yes and that Mode is set to Enforced.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.3.4 Ensure all member users are 'MFA capable' (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft defines Multifactor authentication capable as being registered and enabled for a strong authentication method.

#### Configuration

1. [ ] Remediation steps will depend on the status of the personnel in question or configuration of Conditional Access policies and will not be covered in detail. Administrators should review each user identified on a case-by-case basis using the conditions below. User has never signed on:
2. [ ] Employment status should be reviewed, and appropriate action taken on the user account's roles, licensing and enablement. Conditional Access policy applicability:
3. [ ] Ensure a CA policy is in place requiring all users to use MFA.
4. [ ] Ensure the user is not excluded from the CA MFA policy.
5. [ ] Ensure the policy's state is set to On.
6. [ ] Use What if to determine applicable CA policies. (Protection > Conditional Access > Policies)
7. [ ] Review the user account in Sign-in logs. Under the Activity Details pane click the Conditional Access tab to view applied policies. Note: Conditional Access is covered step by step in section 5.2.2

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select User registration details.
3. [ ] Set the filter option Multifactor authentication capable to Not Capable.
4. [ ] Review the non-guest users in this list.
5. [ ] Excluding any exceptions users found in this report may require remediation.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.3.5 Ensure weak authentication methods are disabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Authentication methods support a wide variety of scenarios for signing in to Microsoft 365 resources.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select Policies.
3. [ ] Inspect each method that is out of compliance and remediate: o Click on the method to open it. o Change the Enable toggle to the off position. o Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select Policies.
3. [ ] Verify that the following methods in the Enabled column are set to No. o Method: SMS o Method: Voice call

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.3.6 Ensure system-preferred multifactor authentication is enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** System-preferred multifactor authentication (MFA) prompts users to sign in by using the most secure method they registered.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select Settings.
3. [ ] Set the System-preferred multifactor authentication State to Enabled and include All users.
4. [ ] Any users exclusions should be documented and reviewed annually.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select Settings.
3. [ ] Verify the System-preferred multifactor authentication State is set to Enabled and All users are included.
4. [ ] Verify that only documented exclusions exist and that they are reviewed annually

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.3.8 Ensure that Account 'Lockout threshold' is '10' or less (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The account lockout threshold determines how many failed login attempts are permitted prior to placing the account in a locked-out state and initiating a variable lockout duration.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select Password protection.
3. [ ] Set Lockout threshold to 10 or less.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select Password protection.
3. [ ] Verify that Lockout threshold is set to 10 or less.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.3.9 Ensure that Account 'Lockout duration in seconds' is at least 60 seconds (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The account lockout duration value determines how long an account retains the status of lockout, and therefore how long before a user can continue to attempt to login after passing the lockout threshold.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select Password protection.
3. [ ] Set the Lockout duration in seconds to 60 or higher.
4. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Authentication methods and select Password protection.
3. [ ] Verify that Lockout duration in seconds is set to 60 or higher.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.3.10 Ensure Microsoft Authenticator on companion applications is disabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Entra ID includes a feature called Authenticator Lite, which embeds a subset of Microsoft Authenticator functionality into companion applications such as Outlook mobile.

#### Configuration

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Authentication methods and select Policies.
3. [ ] Under Method select Microsoft Authenticator.
4. [ ] Select Configure.
5. [ ] Set Microsoft Authenticator on companion applications: Status to Disabled.
6. [ ] Select Save.

#### Validation and evidence

1. [ ] Navigate to the Microsoft Entra admin center https://entra.microsoft.com.
2. [ ] Expand Entra ID > Authentication methods and select Policies.
3. [ ] Under Method select Microsoft Authenticator.
4. [ ] Select Configure.
5. [ ] Verify that Microsoft Authenticator on companion applications: Status is set to Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.4.1 Ensure 'Self service password reset enabled' is set to 'All' (Manual)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Enabling self-service password reset allows users to reset their own passwords in Entra ID.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Password reset and select Properties.
3. [ ] Set Self service password reset enabled to All

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Password reset and select Properties.
3. [ ] Verify that Self service password reset enabled is set to All

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.4.3 Ensure SSPR registration and authentication re- confirmation are required (Manual)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The Require users to register when signing in?

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Password reset and select Registration.
3. [ ] Set Require users to register when signing in? to Yes.
4. [ ] Set Number of days before users are asked to re-confirm their authentication information to any organization-approved value other than 0.
5. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Password reset and select Registration.
3. [ ] Verify that Require users to register when signing in? is set to Yes.
4. [ ] Verify that Number of days before users are asked to re-confirm their authentication information is not set to 0.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.4.4 Ensure that users are notified on password resets (Manual)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting determines whether or not users receive an email to their primary and alternate email addresses notifying them when their own password has been reset via the Self-Service Password Reset portal.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Password reset and select Notifications.
3. [ ] Set Notify users on password resets? to Yes
4. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Password reset and select Notifications.
3. [ ] Verify that Notify users on password resets? is set to Yes.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.2.4.5 Ensure all admins are notified when other admins reset their password (Manual)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting determines whether or not all global administrators receive an email to their primary email address when other administrators reset their own passwords via the Self-Service Password Reset Portal.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Password reset and select Notifications.
3. [ ] Set Notify all admins when other admins reset their password? to Yes
4. [ ] Click Save

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand Entra ID > Password reset and select Notifications.
3. [ ] Verify that Notify all admins when other admins reset their password? is set to Yes

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.3.2 Ensure 'Access reviews' for guest users are configured (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Access reviews enable administrators to establish an efficient automated process for reviewing group memberships, access to enterprise applications, and role assignments.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand ID Governance and select Access reviews
3. [ ] Click New access review.
4. [ ] In the Resource review box click Select.
5. [ ] In Review Type set the following: o Select what to review choose Teams + Groups. o Review Scope to All Microsoft 365 groups with guest users. o Scope to Guest users only then click Next: Reviews.
6. [ ] In Reviews set the following: o Select reviewers to Group members or Selected users and groups, ensuring that at least one reviewer is assigned and that the guest is not performing a self-review. o Duration (in days) to 14 days or less. o Review recurrence to Monthly or more frequent. o Start date for the review, ensuring the review becomes active before the next audit date. o End to Never, then click Next: Settings.
7. [ ] In Settings set the following: o Auto apply results to resource is checked. o If reviewers don't respond to Remove access o Justification required is checked. o E-mail notifications is checked. o Reminders is checked. o Click Next: Review + Create
8. [ ] Click Create.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand ID Governance and select Access reviews
3. [ ] Inspect the access reviews, and verify an access review is created with the following criteria: o Overview: Scope is set to Guest users only and Review status is Active o Reviewers: At least one reviewer is assigned, and the reviewer is not a guest user. o Settings > General: ▪ Mail notifications is set to Enable ▪ Reminders is set to Enable o Settings > Reviewers: ▪ Require reason on approval is set to Enable o Settings > Scheduling: ▪ Frequency is set to Monthly or more frequent ▪ Duration (in days) does not exceed 14 days ▪ End is set to Never o Settings > When completed: ▪ Auto apply results to resource is set to Enable ▪ If reviewers don't respond is set to Remove access
4. [ ] The control is compliant if there is at least one access review for guests that meets all criteria above.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.3.3 Ensure 'Access reviews' for privileged roles are configured (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Access reviews in Microsoft Entra Privileged Identity Management (PIM) enable administrators to periodically validate whether users still require their privileged role assignments.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand ID Governance > Privileged Identity Management.
3. [ ] Select Microsoft Entra Roles under Manage.
4. [ ] Select Access reviews and click New. o Provide a name and description. o Set Frequency to Monthly or more frequently. o Set Duration (in days) to at most 14. o Set End to Never. o Set Users scope to All users and groups. o In Role select the directory roles outlined in the Additional Information section. o Set Assignment type to All active and eligible assignments. o Set Reviewers to member(s) responsible for this type of review, other than self.
5. [ ] In Upon completion settings set the following: o Auto apply results to resource to Enable. o If reviewers don't respond to No change.
6. [ ] In Advanced settings set the following: o Require reason on approval to Enable o Mail notifications to Enable o Reminders to Enable
7. [ ] Click Start to save and begin the review series. Warning: Care should be taken when configuring the If reviewers don't respond setting for Global Administrator reviews, if misconfigured break-glass accounts could automatically have roles revoked. Additionally, reviewers should be educated on the purpose of break-glass accounts to prevent accidental manual removal of roles.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/
2. [ ] Expand ID Governance > Privileged Identity Management.
3. [ ] Select Microsoft Entra Roles under Manage.
4. [ ] Select Access reviews
5. [ ] For each privileged role listed in the Additional Information section, verify an access review exists that meets the following criteria: o Overview: ▪ Role assignment type is set to Eligible and Active ▪ Scope is set to Everyone ▪ Review status is Active o Reviewers: At least one reviewer is assigned, and the reviewer is not self- reviewing. o Settings > General: ▪ Mail notifications is set to Enable ▪ Reminders is set to Enable o Settings > Reviewers: ▪ Require reason on approval is set to Enable o Settings > Scheduling: ▪ Frequency is set to Monthly or more frequently ▪ Duration (in days) does not exceed 14 days ▪ End is set to Never o Settings > When completed: ▪ Auto apply results to resource is set to Enable ▪ If reviewers don't respond is set to No change

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.3.4 Ensure approval is required for Global Administrator role activation (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Entra Privileged Identity Management can be used to audit roles, allow just in time activation of roles and allow for periodic role attestation.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand ID Governance > Privileged Identity Management.
3. [ ] Under Manage select Microsoft Entra Roles.
4. [ ] Under Manage select Roles.
5. [ ] Select Global Administrator in the list.
6. [ ] Select Role settings and click Edit.
7. [ ] Check the Require approval to activate box.
8. [ ] Add at least one approver.
9. [ ] Click Update.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand ID Governance > Privileged Identity Management.
3. [ ] Under Manage select Microsoft Entra Roles.
4. [ ] Under Manage select Roles.
5. [ ] Select Global Administrator in the list.
6. [ ] Select Role settings.
7. [ ] Verify that Require approval to activate is set to Yes.
8. [ ] Verify there is at least 1 approvers in the list.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 5.3.5 Ensure approval is required for Privileged Role Administrator activation (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Microsoft Entra Privileged Identity Management can be used to audit roles, allow just in time activation of roles and allow for periodic role attestation.

#### Configuration

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand ID Governance > Privileged Identity Management.
3. [ ] Under Manage select Microsoft Entra Roles.
4. [ ] Under Manage select Roles.
5. [ ] Select Privileged Role Administrator in the list.
6. [ ] Select Role settings and click Edit.
7. [ ] Check the Require approval to activate box.
8. [ ] Add at least one approver.
9. [ ] Click Update.

#### Validation and evidence

1. [ ] Navigate to Microsoft Entra admin center https://entra.microsoft.com/.
2. [ ] Expand ID Governance > Privileged Identity Management.
3. [ ] Under Manage select Microsoft Entra Roles.
4. [ ] Under Manage select Roles.
5. [ ] Select Privileged Role Administrator in the list.
6. [ ] Select Role settings.
7. [ ] Verify Require approval to activate is set to Yes.
8. [ ] Verify there is at least one approvers in the list.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

## 6. Exchange Online

### 6.1.1 Ensure 'AuditDisabled' organizationally is set to 'False' (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The value False indicates that mailbox auditing on by default is turned on for the organization.

#### Configuration

1. [ ] To remediate using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] Run the following PowerShell command: Set-OrganizationConfig -AuditDisabled $false

#### Validation and evidence

1. [ ] To audit using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] Run the following PowerShell command: Get-OrganizationConfig | Format-List AuditDisabled
4. [ ] Verify that AuditDisabled is set to False.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 6.1.2 Ensure mailbox audit actions are configured (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Mailbox audit logging is turned on by default in all organizations.

#### Configuration

1. [ ] For each UserMailbox ensure AuditEnabled is True and the following audit actions are included in addition to default actions of each sign-in type.
2. [ ] Admin actions: Copy, FolderBind and Move.
3. [ ] Delegate actions: FolderBind and Move.
4. [ ] Owner actions: Create, MailboxLogin and Move. Note: The defaults can be found in the Default Value section and the combined total can be found in the scripts of the Audit/Remediation sections. To remediate using PowerShell:
5. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
6. [ ] Run the following PowerShell script to remediate every 'UserMailbox' in the organization: $AuditAdmin = @( "ApplyRecord", "Copy", "Create", "FolderBind", "HardDelete", "MailItemsAccessed", "Move", "MoveToDeletedItems", "SendAs", "SendOnBehalf", "Send", "SoftDelete", "Update", "UpdateCalendarDelegation", "UpdateFolderPermissions", "UpdateInboxRules" ) $AuditDelegate = @( "ApplyRecord", "Create", "FolderBind", "HardDelete", "Move", "MailItemsAccessed", "MoveToDeletedItems", "SendAs", "SendOnBehalf", "SoftDelete", "Update", "UpdateFolderPermissions", "UpdateInboxRules" ) $AuditOwner = @( "ApplyRecord", "Create", "HardDelete", "MailboxLogin", "Move", "MailItemsAccessed", "MoveToDeletedItems", "Send", "SoftDelete", "Update", "UpdateCalendarDelegation", "UpdateFolderPermissions", "UpdateInboxRules" ) $MBX = Get-EXOMailbox -ResultSize Unlimited | Where-Object { $_.RecipientTypeDetails -eq "UserMailbox" } $MBX | Set-Mailbox -AuditEnabled $true ` -AuditLogAgeLimit 180 -AuditAdmin $AuditAdmin -AuditDelegate $AuditDelegate ` -AuditOwner $AuditOwner
7. [ ] The script will apply the prescribed Audit Actions for each sign-in type (Owner, Delegate, Admin) and the AuditLogAgeLimit to each UserMailbox in the organization. Note: Mailboxes with Audit (Premium) licenses, which is included with E5, can retain audit logs beyond 180 days.

#### Validation and evidence

1. [ ] Inspect each UserMailbox and ensure AuditEnabled is True and the following audit actions are included in addition to default actions of each sign-in type.
2. [ ] Admin actions: Copy, FolderBind and Move.
3. [ ] Delegate actions: FolderBind and Move.
4. [ ] Owner actions: Create, MailboxLogin and Move. Note: The defaults can be found in the Default Value section and the combined total can be found in the scripts of the Audit/Remediation sections. To audit using PowerShell:
5. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
6. [ ] Run the following PowerShell script: $AdminActions = @( "ApplyRecord", "Copy", "Create", "FolderBind", "HardDelete", "MailItemsAccessed", "Move", "MoveToDeletedItems", "SendAs", "SendOnBehalf", "Send", "SoftDelete", "Update", "UpdateCalendarDelegation", "UpdateFolderPermissions", "UpdateInboxRules" ) $DelegateActions = @( "ApplyRecord", "Create", "FolderBind", "HardDelete", "Move", "MailItemsAccessed", "MoveToDeletedItems", "SendAs", "SendOnBehalf", "SoftDelete", "Update", "UpdateFolderPermissions", "UpdateInboxRules" ) $OwnerActions = @( "ApplyRecord", "Create", "HardDelete", "MailboxLogin", "Move", "MailItemsAccessed", "MoveToDeletedItems", "Send", "SoftDelete", "Update", "UpdateCalendarDelegation", "UpdateFolderPermissions", "UpdateInboxRules" ) function VerifyActions { param ( [array]$ExpectedActions, [array]$ActualActions ) $Missing = $ExpectedActions | Where-Object { $_ -notin $ActualActions } return $Missing } $MBX = Get-EXOMailbox -PropertySets Audit, Minimum -ResultSize Unlimited | Where-Object { $_.RecipientTypeDetails -eq "UserMailbox" } $Results = foreach ($mailbox in $MBX) { $AdminMissing = VerifyActions -ExpectedActions $AdminActions ` -ActualActions $mailbox.AuditAdmin $DelegateMissing = VerifyActions -ExpectedActions $DelegateActions ` -ActualActions $mailbox.AuditDelegate $OwnerMissing = VerifyActions -ExpectedActions $OwnerActions ` -ActualActions $mailbox.AuditOwner $IsCompliant = $AdminMissing.Count -eq 0 -and $DelegateMissing.Count -eq 0 -and $OwnerMissing.Count -eq 0 -and $mailbox.AuditEnabled [PSCustomObject]@{ Mailbox = $mailbox.UserPrincipalName AuditEnabled = $mailbox.AuditEnabled AdminMissing = if ($AdminMissing.Count -gt 0) { $AdminMissing -join ", " } else { "None" } DelegateMissing = if ($DelegateMissing.Count -gt 0) { $DelegateMissing -join ", " } else { "None" } OwnerMissing = if ($OwnerMissing.Count -gt 0) { $OwnerMissing -join ", " } else { "None" } ComplianceState = if ($IsCompliant) { "Compliant" } else { "Non-Compliant" } } } # Display results in table format $Results | Format-Table -AutoSize <# Optional: Export methods $Results | Out-GridView -Title "Mailbox Audit Results" $Results | Export-Csv -Path "6.1.2.csv" -NoTypeInformation $Results | ConvertTo-Json | Out-File -FilePath "6.1.2.json" #>
7. [ ] Inspect the results. Mailboxes will be labeled as either Compliant or Non- compliant, accompanied by supporting details that outline the missing actions for each type and the current state of AuditEnabled. Optional methods for exporting the data to CSV, JSON, or GridView are also shown at the end of the script. Note: Mailboxes with Audit (Premium) licenses, which is included with E5, can retain audit logs beyond 180 days.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 6.1.3 Ensure 'AuditBypassEnabled' is not enabled on mailboxes (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** When configuring a user or computer account to bypass mailbox audit logging, the system will not record any access, or actions performed by the said user or computer account on any mailbox.

#### Configuration

1. [ ] To remediate using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] The following example PowerShell script will disable AuditBypass for all mailboxes which currently have it enabled: # Get mailboxes with AuditBypassEnabled set to $true $MBXAudit = Get-MailboxAuditBypassAssociation -ResultSize unlimited | Where- Object { $_.AuditBypassEnabled -eq $true } foreach ($mailbox in $MBXAudit) { $mailboxName = $mailbox.Name Set-MailboxAuditBypassAssociation -Identity $mailboxName - AuditBypassEnabled $false Write-Host "Audit Bypass disabled for mailbox Identity: $mailboxName" - ForegroundColor Green }

#### Validation and evidence

1. [ ] To audit using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] Run the following PowerShell command: $MBXData = Get-MailboxAuditBypassAssociation -ResultSize unlimited $Report = $MBXData | ? {$_.AuditBypassEnabled -eq $true} | select Name,AuditBypassEnabled $Report <# Optional: Export methods $Report | Out-GridView -Title "Mailbox Audit Bypass Association" $Report | Export-Csv -Path "6.1.3.csv" -NoTypeInformation #>
4. [ ] If nothing is returned, then there are no accounts with Audit Bypass enabled. Note: The cmdlet Get-MailboxAuditBypassAssociation may display a WARNING on system objects that begin with "Asc-2X1", this is not part of the Audit procedure and can be ignored.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 6.2.1 Ensure all forms of mail forwarding are blocked and/or disabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Exchange Online offers several methods of managing the flow of email messages.

#### Configuration

1. [ ] Select Exchange to open the Exchange admin center.
2. [ ] Select Mail Flow then Rules.
3. [ ] For each rule that redirects email to external domains, select the rule and click the 'Delete' icon.

#### Validation and evidence

1. [ ] Select Exchange to open the Exchange admin center.
2. [ ] Select Mail Flow then Rules.
3. [ ] Review the rules and verify that none of them are forwards or redirects e-mail to external domains.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 6.2.2 Ensure mail transport rules do not whitelist specific domains (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Mail flow rules (transport rules) in Exchange Online can be configured to set the spam confidence level (SCL) of a message to -1, which bypasses spam and phishing filtering.

#### Configuration

1. [ ] Navigate to Exchange admin center https://admin.exchange.microsoft.com
2. [ ] Click to expand Mail Flow and then select Rules.
3. [ ] For each rule that sets the spam confidence level to -1 for a specific domain, select the rule and click Delete.

#### Validation and evidence

1. [ ] Navigate to Exchange admin center https://admin.exchange.microsoft.com
2. [ ] Click to expand Mail Flow and then select Rules.
3. [ ] Review each rule and ensure that a single rule does not contain both of these properties together: o Under Apply this rule if: Sender's address domain portion belongs to any of these domains: '<domain>' o Under Do the following: Set the spam confidence level (SCL) to '-1'

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 6.2.3 Ensure email from external senders is identified (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** External callouts provide a native experience to identify emails from senders outside the organization.

#### Configuration

1. [ ] To remediate using PowerShell:
2. [ ] Connect to Exchange online using Connect-ExchangeOnline.
3. [ ] Run the following PowerShell command: Set-ExternalInOutlook -Enabled $true

#### Validation and evidence

1. [ ] To audit using PowerShell:
2. [ ] Connect to Exchange online using Connect-ExchangeOnline.
3. [ ] Run the following PowerShell command: Get-ExternalInOutlook
4. [ ] For each identity verify Enabled is set to True and the AllowList only contains email addresses the organization has permitted to bypass external tagging.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 6.3.2 Ensure the ability to add personal email accounts and calendars is disabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Outlook on the web (OWA) mailbox policies include two settings that control personal account integration in Outlook.

#### Configuration

1. [ ] To remediate using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] Run the following: $DefaultPolicy = Get-OwaMailboxPolicy | Where-Object { $_.IsDefault } Set-OwaMailboxPolicy -Identity $DefaultPolicy.Identity - PersonalAccountsEnabled $false -PersonalAccountCalendarsEnabled $false

#### Validation and evidence

1. [ ] Note: The default OWA Mailbox Policy is the only policy required for compliance with this control. Other mailbox policies are discretionary and left up to the organization to audit as needed. To audit using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] Run the following: Get-OwaMailboxPolicy | Where-Object { $_.IsDefault } | Format-List PersonalAccountsEnabled, PersonalAccountCalendarsEnabled
4. [ ] Verify the output matches the following: PersonalAccountsEnabled : False PersonalAccountCalendarsEnabled : False

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 6.5.1 Ensure modern authentication for Exchange Online is enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Modern authentication in Microsoft 365 enables authentication features like multifactor authentication (MFA) using smart cards, certificate-based authentication (CBA), and third-party SAML identity providers.

#### Configuration

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Settings and select Org Settings.
3. [ ] Select Modern authentication.
4. [ ] Check Turn on modern authentication for Outlook 2013 for Windows and later (recommended) to enable modern authentication.

#### Validation and evidence

1. [ ] Navigate to Microsoft 365 admin center https://admin.microsoft.com.
2. [ ] Expand Settings and select Org Settings.
3. [ ] Select Modern authentication.
4. [ ] Verify that Turn on modern authentication for Outlook 2013 for Windows and later (recommended) is checked.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 6.5.2 Ensure MailTips are enabled for end users (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** MailTips are informative messages displayed to users while they're composing a message.

#### Configuration

1. [ ] To remediate using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] Run the following PowerShell command: $TipsParams = @{ MailTipsAllTipsEnabled = $true MailTipsExternalRecipientsTipsEnabled = $true MailTipsGroupMetricsEnabled = $true MailTipsLargeAudienceThreshold = '25' } Set-OrganizationConfig @TipsParams

#### Validation and evidence

1. [ ] To audit using PowerShell:
2. [ ] Connect to Exchange Online using Connect-ExchangeOnline.
3. [ ] Run the following PowerShell command: Get-OrganizationConfig | fl MailTips*
4. [ ] Verify the values for MailTipsAllTipsEnabled, MailTipsExternalRecipientsTipsEnabled, and MailTipsGroupMetricsEnabled are set to True and MailTipsLargeAudienceThreshold is set to an acceptable value; 25 is the default value.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 6.5.4 Ensure SMTP AUTH is disabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting enables or disables authenticated client SMTP submission (SMTP AUTH) at an organization level in Exchange Online.

#### Configuration

1. [ ] Navigate to Exchange admin center https://admin.exchange.microsoft.com.
2. [ ] Expand Settings and select Mail flow.
3. [ ] Check Turn off SMTP AUTH protocol for your organization to disable the protocol.

#### Validation and evidence

1. [ ] Navigate to Exchange admin center https://admin.exchange.microsoft.com.
2. [ ] Expand Settings and select Mail flow.
3. [ ] Ensure Turn off SMTP AUTH protocol for your organization is checked.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

## 7. SharePoint Online and OneDrive

### 7.2.1 Ensure modern authentication for SharePoint applications is required (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Modern authentication in Microsoft 365 enables authentication features like multifactor authentication (MFA) using smart cards, certificate-based authentication (CBA), and third-party SAML identity providers.

#### Configuration

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint.
2. [ ] Expand Policies and select Access control.
3. [ ] Select Apps that don't use modern authentication.
4. [ ] Select the radio button for Block access.
5. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint.
2. [ ] Expand Policies and select Access control.
3. [ ] Select Apps that don't use modern authentication and ensure that it is set to Block access.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 7.2.2 Ensure SharePoint and OneDrive integration with Azure AD B2B is enabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Entra ID B2B provides authentication and management of guests.

#### Configuration

1. [ ] To remediate using PowerShell:
2. [ ] Connect to SharePoint Online using Connect-SPOService
3. [ ] Run the following command: Set-SPOTenant -EnableAzureADB2BIntegration $true

#### Validation and evidence

1. [ ] To audit using PowerShell:
2. [ ] Connect to SharePoint Online using Connect-SPOService
3. [ ] Run the following command: Get-SPOTenant | ft EnableAzureADB2BIntegration
4. [ ] Verify that the returned value is True.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 7.2.3 Ensure external content sharing is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** The external sharing settings govern sharing for the organization overall.

#### Configuration

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Locate the External sharing section.
4. [ ] Under SharePoint, move the slider bar to New and existing guests or a less permissive level. o OneDrive will also be moved to the same level and can never be more permissive than SharePoint.

#### Validation and evidence

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Locate the External sharing section.
4. [ ] Under SharePoint, verify that the slider bar is set to New and existing guests or a less permissive level.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 7.2.7 Ensure link sharing is restricted in SharePoint and OneDrive (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting sets the default link type that a user will see when sharing content in OneDrive or SharePoint.

#### Configuration

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Scroll to File and folder links.
4. [ ] Set Choose the type of link that's selected by default when users share files and folders in SharePoint and OneDrive to Specific people (only the people the user specifies) or Only people in your organization.

#### Validation and evidence

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Scroll to File and folder links.
4. [ ] Verify that the setting Choose the type of link that's selected by default when users share files and folders in SharePoint and OneDrive is set to Specific people (only the people the user specifies) or Only people in your organization.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 7.2.9 Ensure guest access to a site or OneDrive will expire automatically (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This policy setting configures the expiration time for each guest that is invited to the SharePoint site or with whom users share individual files and folders with.

#### Configuration

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Scroll to and expand More external sharing settings.
4. [ ] Set Guest access to a site or OneDrive will expire automatically after this many days to 30

#### Validation and evidence

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Scroll to and expand More external sharing settings.
4. [ ] Verify that Guest access to a site or OneDrive will expire automatically after this many days is checked and set to 30.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 7.2.10 Ensure reauthentication with verification code is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting configures if guests who use a verification code to access the site or links are required to reauthenticate after a set number of days.

#### Configuration

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Scroll to and expand More external sharing settings.
4. [ ] Set People who use a verification code must reauthenticate after this many days to 15 or less.

#### Validation and evidence

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Scroll to and expand More external sharing settings.
4. [ ] Verify that People who use a verification code must reauthenticate after this many days is set to 15 or less.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 7.2.11 Ensure the SharePoint default sharing link permission is set (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting configures the permission that is selected by default for sharing link from a SharePoint site.

#### Configuration

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Scroll to File and folder links.
4. [ ] Set Choose the permission that's selected by default for sharing links to View.

#### Validation and evidence

1. [ ] Navigate to SharePoint admin center https://admin.microsoft.com/sharepoint
2. [ ] Expand Policies > Sharing.
3. [ ] Scroll to File and folder links.
4. [ ] Verify that Choose the permission that's selected by default for sharing links is set to View.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

## 8. Microsoft Teams

### 8.1.2 Ensure users can't send emails to a channel email address (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting controls whether Teams channels are allowed to receive emails sent to their unique email addresses.

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Select Settings & policies > Global (Org-wide default) settings.
3. [ ] Click Teams to open the Teams settings section.
4. [ ] Under email integration set Users can send emails to a channel email address to Off.

#### Validation and evidence

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Select Settings & policies > Global (Org-wide default) settings.
3. [ ] Click Teams to open the Teams settings section.
4. [ ] Under email integration verify that Users can send emails to a channel email address is Off.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 8.2.2 Ensure communication with unmanaged Teams users is disabled (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This policy setting controls chats and meetings initiated through the external access channel with unmanaged Teams users (those not managed by an organization, such as Microsoft Teams (free)).

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com/.
2. [ ] Expand External collaboration and select External access.
3. [ ] Open the Policies tab.
4. [ ] Click on the Global (Org-wide default) settings policy.
5. [ ] Set People in my org can chat and have meetings with external users who have unmanaged Microsoft accounts to Off.
6. [ ] Click Save.

#### Validation and evidence

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com/.
2. [ ] Expand External collaboration and select External access.
3. [ ] Open the Policies tab.
4. [ ] Click on the Global (Org-wide default) settings policy.
5. [ ] Verify that People in my org can chat and have meetings with external users who have unmanaged Microsoft accounts is set to Off.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 8.2.3 Ensure external Teams users cannot initiate conversations (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting prevents external users who are not managed by an organization from initiating contact with users in the protected organization.

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com/.
2. [ ] Expand External collaboration and select External access.
3. [ ] Open the Policies tab.
4. [ ] Click on the Global (Org-wide default) settings policy.
5. [ ] Locate the parent setting People in my org can chat and have meetings with external users who have unmanaged Microsoft accounts.
6. [ ] Uncheck People in my org can join external meetings and receive new chats from users who have unmanaged Microsoft accounts.
7. [ ] Click Save.

#### Validation and evidence

1. [ ] Note: If the parent setting People in my org can chat and have meetings with external users who have unmanaged Microsoft accounts is already set to Off then this setting will not be visible in the UI.
2. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com/.
3. [ ] Expand External collaboration and select External access.
4. [ ] Open the Policies tab.
5. [ ] Click on the Global (Org-wide default) settings policy.
6. [ ] Locate the parent setting People in my org can chat and have meetings with external users who have unmanaged Microsoft accounts.
7. [ ] Verify that People in my org can join external meetings and receive new chats from users who have unmanaged Microsoft accounts is not checked.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 8.2.4 Ensure the organization cannot communicate with accounts in trial Teams tenants (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting controls the organization's external access with Teams "trial-only" tenants.

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com/.
2. [ ] Expand External collaboration and select External access.
3. [ ] Select the Organization settings tab.
4. [ ] Set People in my organization can communicate with accounts in trial Teams tenant to Off.

#### Validation and evidence

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com/.
2. [ ] Expand External collaboration and select External access.
3. [ ] Select the Organization settings tab.
4. [ ] Verify that People in my organization can communicate with accounts in trial Teams tenant is set to Off.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 8.4.1 Ensure app permission policies are configured (Manual)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This policy setting controls which class of apps are available for users to install.

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Expand Teams apps and select Manage apps.
3. [ ] In the upper right click Actions > Org-wide app settings.
4. [ ] For Third-party apps set Let users install and use available apps by default to Off.
5. [ ] For Custom apps set Let users install and use available apps by default to Off.
6. [ ] For Custom apps set Let users interact with custom apps in preview to Off.

#### Validation and evidence

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Expand Teams apps and select Manage apps.
3. [ ] In the upper right click Actions > Org-wide app settings.
4. [ ] For Third-party apps verify Let users install and use available apps by default is Off.
5. [ ] For Custom apps verify Let users install and use available apps by default is Off.
6. [ ] For Custom apps verify Let users interact with custom apps in preview is Off.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 8.5.2 Ensure anonymous users and dial-in callers can't start a meeting (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This policy setting controls if an anonymous participant can start a Microsoft Teams meeting without someone in attendance.

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Meetings to open the meeting settings section.
4. [ ] Under meeting join & lobby set Anonymous users and dial-in callers can start a meeting to Off.

#### Validation and evidence

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Meetings to open the meeting settings section.
4. [ ] Under meeting join & lobby verify that Anonymous users and dial-in callers can start a meeting is set to Off.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 8.5.3 Ensure only people in my org can bypass the lobby (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This policy setting controls who can join a meeting directly and who must wait in the lobby until they're admitted by an organizer, co-organizer, or presenter of the meeting.

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Meetings to open the meeting settings section.
4. [ ] Under meeting join & lobby set Who can bypass the lobby to one of the following: o People who were invited o People in my org o Only organizers and co-organizers

#### Validation and evidence

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Meetings to open the meeting settings section.
4. [ ] Under meeting join & lobby verify Who can bypass the lobby is set to one of the following: o People who were invited o People in my org o Only organizers and co-organizers

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 8.5.4 Ensure users dialing in can't bypass the lobby (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This policy setting controls if users who dial in by phone can join the meeting directly or must wait in the lobby.

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Meetings to open the meeting settings section.
4. [ ] Under meeting join & lobby set People dialing in can bypass the lobby to Off.

#### Validation and evidence

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Meetings to open the meeting settings section.
4. [ ] Under meeting join & lobby verify that People dialing in can bypass the lobby is set to Off.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 8.5.7 Ensure external participants can't give or request control (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This policy setting allows control of who can present in meetings and who can request control of the presentation while a meeting is underway.

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Meetings to open the meeting settings section.
4. [ ] Under content sharing set External participants can give or request control to Off.

#### Validation and evidence

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Meetings to open the meeting settings section.
4. [ ] Under content sharing verify that External participants can give or request control is Off.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 8.6.1 Ensure users can report security concerns in Teams (Automated)

**Profiles:** E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** User reporting settings allow a user to report a message as malicious for further analysis.

#### Configuration

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Messaging to open the messaging settings section.
4. [ ] Set Report a security concern to On.
5. [ ] Next, navigate to Microsoft 365 Defender https://security.microsoft.com/
6. [ ] Expand System > Settings and select Email & collaboration.
7. [ ] Click on User reported settings.
8. [ ] Under Microsoft Teams check the box for Monitor reported items in Microsoft Teams and click Save.
9. [ ] Set Send reported messages to: to My reporting mailbox only with reports configured to be sent to authorized staff.

#### Validation and evidence

1. [ ] Navigate to Microsoft Teams admin center https://admin.teams.microsoft.com.
2. [ ] Click Settings & policies and select the Global (Org-wide default) settings tab.
3. [ ] Select Messaging to open the messaging settings section.
4. [ ] Verify that Report a security concern is On.
5. [ ] Next, navigate to Microsoft 365 Defender https://security.microsoft.com/
6. [ ] Expand System > Settings and select Email & collaboration.
7. [ ] Click on User reported settings.
8. [ ] Under Microsoft Teams verify that Monitor reported items in Microsoft Teams is checked.
9. [ ] Verify that Send reported messages to: is set to My reporting mailbox only with report email addresses defined for authorized staff.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

## 9. Power Platform and Fabric

### 9.1.1 Ensure guest user access is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting allows business-to-business (B2B) guests access to Microsoft Fabric, and contents that they have permissions to.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Set Guest users can access Microsoft Fabric to one of these states: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Verify that Guest users can access Microsoft Fabric is set to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.2 Ensure external user invitations are restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting helps organizations choose whether new external users can be invited to the organization through Power BI sharing, permissions, and subscription experiences.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Set Users can invite guest users to collaborate through item sharing and permissions to one of these states: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Verify that Users can invite guest users to collaborate through item sharing and permissions is set to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.3 Ensure guest access to content is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting allows Microsoft Entra B2B guest users to have full access to the browsing experience using the left-hand navigation pane in the organization.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Set Guest users can browse and access Fabric content to one of these states: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Verify that Guest users can browse and access Fabric content is set to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.4 Ensure 'Publish to web' is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Power BI enables users to share reports and materials directly on the internet from both the application's desktop version and its web user interface.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Set Publish to web to one of these states: o Disabled o Enabled with Choose how embed codes work set to Only allow existing codes AND Specific security groups selected and defined Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Verify that Publish to web is set to one of the following: o Disabled o Enabled with Choose how embed codes work set to Only allow existing codes AND Specific security groups selected and defined Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.6 Ensure 'Allow users to apply sensitivity labels for content' is 'Enabled' (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Information protection tenant settings help to protect sensitive information in the Power BI tenant.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Information protection.
4. [ ] Set Allow users to apply sensitivity labels for content to one of these states: o Enabled o Enabled with Specific security groups selected and defined.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Information protection.
4. [ ] Verify that Allow users to apply sensitivity labels for content is set to one of the following: o Enabled o Enabled with Specific security groups selected and defined.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.7 Ensure shareable links are restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Creating a shareable link allows a user to create a link to a report or dashboard, then add that link to an email or another messaging application.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Set Allow shareable links to grant access to everyone in your organization to one of these states: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Verify that Allow shareable links to grant access to everyone in your organization is set to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.8 Ensure enabling of external data sharing is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Power BI admins can specify which users or user groups can share datasets externally with guests from a different tenant through the in-place mechanism.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Set Allow specific users to turn on external data sharing to one of these states: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Export and Sharing settings.
4. [ ] Verify that Allow specific users to turn on external data sharing is set to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.9 Ensure 'Block ResourceKey Authentication' is 'Enabled' (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** This setting blocks the use of resource key based authentication.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Developer settings.
4. [ ] Set Block ResourceKey Authentication to Enabled

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Developer settings.
4. [ ] Verify that Block ResourceKey Authentication is set to Enabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.10 Ensure access to APIs by service principals is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Use a service principal to access Fabric public APIs that include create, read, update, and delete (CRUD) operations, and are protected by a Fabric permission model.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Developer settings.
4. [ ] Set Service principals can call Fabric public APIs to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Developer settings.
4. [ ] Verify that Service principals can call Fabric public APIs is set to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.11 Ensure service principals cannot create and use profiles (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Service principal profiles provide a flexible solution for apps used in a multitenancy deployment.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Developer settings.
4. [ ] Set Allow service principals to create and use profiles to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Developer settings.
4. [ ] Verify that Allow service principals to create and use profiles is set to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

### 9.1.12 Ensure service principals ability to create workspaces, connections and deployment pipelines is restricted (Automated)

**Profiles:** E3 Level 1, E5 Level 1

**Tracking**

- [ ] Not started
- [ ] In progress
- [ ] Implemented
- [ ] Exception approved
- [ ] Not applicable

**Baseline requirement:** Use a service principal to access these Fabric APIs that aren't protected by a Fabric permission model.

#### Configuration

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Developer settings.
4. [ ] Set Service principals can create workspaces, connections, and deployment pipelines to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

#### Validation and evidence

1. [ ] Navigate to Microsoft Fabric https://app.powerbi.com/admin-portal
2. [ ] Select Tenant settings.
3. [ ] Scroll to Developer settings.
4. [ ] Verify that Service principals can create workspaces, connections, and deployment pipelines is set to one of the following: o Disabled o Enabled with Specific security groups selected and defined. Important: If the organization doesn't actively use this feature it is recommended to keep it Disabled.

- **Owner:**
- **Evidence location:**
- **Implementation notes / exception rationale:**

---

## Enhanced hardening register

Evaluate Level 2 controls for regulated, privileged, internet-facing, or otherwise high-security workloads.

| ID | Control | Profiles | Decision |
|---|---|---|---|
| 1.2.1 | Ensure that only organizationally managed/approved public groups exist (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 1.3.2 | Ensure 'Idle session timeout' is set to '3 hours (or less)' for unmanaged devices (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 1.3.3 | Ensure 'External sharing' of calendars is not available (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 1.3.6 | Ensure the customer lockbox feature is enabled (Automated) | E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 1.3.7 | Ensure 'third-party storage services' are restricted in 'Microsoft 365 on the web' (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 1.3.8 | Ensure that Sways cannot be shared with people outside of your organization (Manual) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 2.1.1 | Ensure Safe Links for Office Applications is Enabled (Automated) | E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 2.1.4 | Ensure Safe Attachments policy is enabled (Automated) | E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 2.1.5 | Ensure Safe Attachments for SharePoint, OneDrive, and Microsoft Teams is Enabled (Automated) | E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 2.1.7 | Ensure that an anti-phishing policy has been created (Automated) | E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 2.1.11 | Ensure comprehensive attachment filtering is applied (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 2.4.3 | Ensure Microsoft Defender for Cloud Apps is enabled and configured (Manual) | E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.2.5 | Ensure the option to remain signed in is hidden (Manual) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.2.6 | Ensure 'LinkedIn account connections' is disabled (Manual) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.3.2 | Ensure that 'Restrict user ability to access groups features in My Groups' is set to 'Yes' (Manual) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.3.4 | Ensure that 'Users can create Microsoft 365 groups in Azure portals, API or PowerShell' is set to 'No' (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.4.1 | Ensure the ability to join devices to Entra is restricted (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.4.6 | Ensure users are restricted from recovering BitLocker keys (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.5.1 | Ensure user consent to apps accessing company data on their behalf is not allowed (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.5.3 | Ensure password addition is blocked for applications (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.6.1 | Ensure that collaboration invitations are sent to allowed domains only (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.1.6.3 | Ensure guest user invitations are limited (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.2.2.5 | Ensure 'Phishing-resistant MFA strength' is required for Administrators (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.2.2.8 | Ensure 'sign-in risk' is blocked for medium and high risk (Automated) | E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.2.2.14 | Ensure trusted 'named locations' are defined (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.2.2.15 | Ensure exclusionary geographic access controls are utilized (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.2.2.16 | Ensure Token Protection is enforced for session tokens (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.2.3.7 | Ensure the email OTP authentication method is disabled (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.2.4.2 | Ensure that 2 methods are required for password reset (Manual) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 5.3.1 | Ensure privileged role assignments are activated and not assigned (Automated) | E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 6.3.1 | Ensure users installing Outlook add-ins is not allowed (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 6.5.3 | Ensure additional storage providers are restricted in Outlook on the web (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 6.5.5 | Ensure Direct Send submissions are rejected (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 7.2.4 | Ensure OneDrive content sharing is restricted (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 7.2.5 | Ensure that SharePoint guest users cannot share items they don't own (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 7.2.6 | Ensure SharePoint external sharing is restricted (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 7.2.8 | Ensure external sharing is restricted by security group (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 7.3.1 | Ensure Office 365 SharePoint infected files are disallowed for download (Automated) | E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 8.1.1 | Ensure external file sharing in Teams is enabled for only approved cloud storage services (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 8.2.1 | Ensure external domains are restricted in the Teams admin center (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 8.5.1 | Ensure anonymous users can't join a meeting (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 8.5.5 | Ensure meeting chat does not allow anonymous users (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 8.5.6 | Ensure only organizers and co-organizers can present (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 8.5.8 | Ensure external meeting chat is off (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 8.5.9 | Ensure meeting recording is off by default (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |
| 9.1.5 | Ensure 'Interact with and share R and Python' visuals is 'Disabled' (Automated) | E3 Level 2, E5 Level 2 | ☐ Adopt / ☐ Defer / ☐ N/A |

## Exception record

| Control ID | Deviation | Compensating control | Owner | Review / expiry |
|---|---|---|---|---|
| | | | | |

## Acceptance

- **Security owner:**
- **Tenant owner:**
- **Implementation lead:**
- **Approval date:**

## Source

- CIS Microsoft 365 Foundations Benchmark v7.0.0 PDF supplied for this project.
- Generated as a GitHub-friendly implementation checklist.
