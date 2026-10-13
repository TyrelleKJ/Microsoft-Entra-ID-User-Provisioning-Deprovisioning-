# Microsoft EntraID User Provisioning, De-provisioning and Configuration 
Light demonstration providing hands on evidence on my ability to proficiently navigate Microsoft 365.


# Microsoft Entra ID Identity Lab

## Overview
This project is a hands-on lab in Microsoft Entra ID (formerly Azure AD), Microsoft's cloud identity and access management service. I built a small test environment to practice core IT administration tasks: creating user accounts, managing sign-in identities, and understanding how access is controlled in a Microsoft cloud tenant. The lab follows Microsoft's SC-300 (Identity and Access Administrator) learning material.

## Environment
- **Platform:** Microsoft Entra admin center (entra.microsoft.com)
- **Tenant:** Default Directory (personal test tenant, test data only)
- **Admin account:** tenant owner account used to create and manage users

## Key Concepts
- **Tenant:** an organization's private identity boundary. All users, groups, and policies live inside it.
- **User principal name (UPN):** the unique sign-in name for each user, in the form `name@domain.onmicrosoft.com`.
- **Member users:** internal accounts created and managed by the organization.
- **Mail nickname:** the email alias, which can be derived automatically from the UPN.
- **Auto-generated password:** a temporary password the user must change at first sign-in.
- **Account enabled:** controls whether an account is allowed to sign in.

## Completed
### Create and manage users
1. Opened Entra ID > Users > All users and confirmed the starting directory (4 users).
2. Selected New user > Create new user.
3. Entered the user principal name, display name, and an auto-generated password, with the account enabled.
4. Reviewed and created the account.
5. Refreshed the user list and verified the new user appeared (5 users).

**Result:** The directory now contains 5 member users, including the new test user, confirming successful account creation.

| Step | Evidence |
|------|----------|
| Starting user list | <img width="1440" height="900" alt="Screenshot 2026-10-13 at 8 15 33 AM" src="https://github.com/user-attachments/assets/fa326d01-9716-40a3-90f0-d3af68b6961d" />
|Create new user form | <img width="1157" height="761" alt="image" src="https://github.com/user-attachments/assets/f2e965c9-4a60-4dd3-8f0a-c12d254c3990" />
| Created User & Viewed Properties | <img width="1440" height="900" alt="Screenshot 2026-10-13 at 8 15 33 AM" src="https://github.com/user-attachments/assets/75f5f191-47c9-4182-b8f7-8a2cb81d4683" /> 
| Updated user list |[<img width="1048" height="703" alt="Screenshot 2026-10-13 at 7 02 48 AM" src="https://github.com/user-attachments/assets/4d3af788-b016-4930-b84d-158f92ce8099" /> ](https://github.com/TyrelleKJ/Microsoft-Entra-ID-User-Provisioning-Deprovisioning-#completed)|
| Screen recording | https://github.com/user-attachments/assets/99c51fb8-a8d3-4010-8a4d-a9778527c4ad |
## What I Learned
- How user identities are created and organized in a cloud tenant.
- Why consistent naming conventions for UPNs and display names matter for managing users at scale.
- That temporary passwords must be captured at creation and changed at first sign-in.
- How the Users list can be used to verify changes immediately.
- How this work maps to everyday help desk tasks like onboarding new employees.

## Future Improvements
This lab covers the foundation of identity management. Planned next steps:
- [ ] **Guest users and external collaboration:** invite outside users and review collaboration settings.
- [ ] **Groups:** create security groups by department and manage membership.
- [ ] **Role-based access control:** assign limited admin roles (for example Helpdesk Administrator) following least privilege.
- [ ] **Self-service password reset (SSPR):** let users reset their own passwords.
- [ ] **Multifactor authentication (MFA):** require a second verification factor.
- [ ] **Conditional Access:** build and test policies, such as requiring MFA for admins.
- [ ] **Monitoring:** review Sign-in logs and Audit logs to verify policy results.
- [ ] **Offboarding:** disable, delete, and restore a user account.
- [ ] **Privileged Identity Management (PIM):** just-in-time admin access with approvals.
- [ ] **Automation:** create users in bulk with CSV upload or PowerShell/Microsoft Graph.

## Resources
- Microsoft Learn: SC-300 Identity and Access Administrator learning path
- GitHub: MicrosoftLearning/SC-300-Identity-and-Access-Administrator
