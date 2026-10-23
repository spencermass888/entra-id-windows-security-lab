# Microsoft Entra ID Access Security and Windows Hardening Lab

## Project Overview

This project explores cloud identity management, sign-in security, and Windows security hardening. The lab uses Microsoft Entra ID to manage test users and departmental security groups, with later phases focused on authentication protections and Windows security settings.

## Part 1: Tenant Setup, Users, and Security Groups

### Overview

In Part 1, I established the Spencer Home Lab tenant, reviewed the available licensing, and created three test users representing IT, HR, and Sales. I created departmental security groups, assigned each user to the appropriate group, and verified the memberships. I then tested each account’s first sign-in and completed the required temporary password changes.

### Technologies Used

- Microsoft Entra ID
- Microsoft 365 admin center
- Microsoft Intune Plan 1 trial
- Microsoft My Account portal

### 1. Verify the Lab Subscription

<img width="1854" height="943" alt="1" src="https://github.com/user-attachments/assets/09a445bf-fc6c-40c3-9cbf-ed989747208f" />

Verified that the Microsoft Intune Plan 1 trial was active, with 25 total licenses, one assigned, and 24 available.

### 2. Review Trial Subscription Settings

<img width="1873" height="941" alt="2" src="https://github.com/user-attachments/assets/b4c451fb-efc4-49ab-b4f4-813678f3f043" />

Reviewed the trial subscription settings, including its expiration date, active subscription status, and confirmation that recurring billing was turned off.

### 3. Review Administrator Licensing

<img width="1872" height="956" alt="3" src="https://github.com/user-attachments/assets/ae788991-7ad2-4461-ac13-9ba3bc4bbab4" />

Confirmed that the administrator account had Microsoft Intune Plan 1 assigned. The available subscription included Intune rather than an Entra ID Premium license.

### 4. Review the Initial Tenant

<img width="1914" height="1019" alt="4" src="https://github.com/user-attachments/assets/1c84c102-faab-4e37-9fd2-b6c0a7c5f4fd" />

Reviewed the Spencer Home Lab tenant before creating the test accounts and groups. The tenant initially contained one user and no groups, and the administrator account held the Global Administrator role.

### 5. Enter ITSupport1 Account Details

<img width="1866" height="913" alt="5" src="https://github.com/user-attachments/assets/49e0d830-bfeb-489a-963c-00e56df643c5" />

Entered ITSupport1’s username and display name, selected an automatically generated temporary password, and left the account enabled.

### 6. Review ITSupport1 Configuration

<img width="1865" height="905" alt="6" src="https://github.com/user-attachments/assets/e8fb5ddf-f425-43a0-9d57-992f1d2f6f14" />

Reviewed ITSupport1’s settings before creating the account. The user was configured as a Member with the IT Support Technician job title, IT department, and United States usage location.

### 7. Verify ITSupport1 Account Creation

<img width="1859" height="915" alt="7" src="https://github.com/user-attachments/assets/f5d3789f-83cb-4a6d-8dfa-f844a3b5889a" />

Confirmed that ITSupport1 was created and enabled, with no assigned administrator roles, applications, or licenses at this stage.

### 8. Enter HRUser1 Account Details

<img width="1850" height="905" alt="8" src="https://github.com/user-attachments/assets/db8e6801-fa00-4072-a29f-e47f6c24915a" />

Entered HRUser1’s username and display name, selected an automatically generated temporary password, and left the account enabled. The password is concealed in the documentation.

### 9. Review HRUser1 Configuration

<img width="1854" height="906" alt="9" src="https://github.com/user-attachments/assets/4a7e36b7-973d-43a8-8397-57024b8616a8" />

Reviewed HRUser1’s settings before creating the account. The user was configured as a Member with the HR Assistant job title and HR department.

### 10. Enter SalesUser1 Account Details

<img width="1855" height="903" alt="10" src="https://github.com/user-attachments/assets/fc612551-0dff-4de4-95a7-dc1dd1ab2c17" />

Entered the initial account details for SalesUser1. The display name shown here was subsequently corrected from Sales Representative to SalesUser1, while Sales Representative was used as the job title.

### 11. Review SalesUser1 Configuration

<img width="1854" height="908" alt="11" src="https://github.com/user-attachments/assets/d7dc6d2e-a52a-447d-8c94-64f5161ce5a6" />

Reviewed the corrected SalesUser1 settings before creating the account. The user was configured as a Member with the Sales Representative job title, Sales department, and United States usage location.

### 12. Verify the Test Users

<img width="1852" height="906" alt="12" src="https://github.com/user-attachments/assets/7c0c7c37-1ee9-40ef-9a89-84c74312d82f" />

Confirmed that ITSupport1, HRUser1, and SalesUser1 appeared in the tenant alongside the administrator account.

### 13. Create the IT Security Group

<img width="1855" height="912" alt="13" src="https://github.com/user-attachments/assets/32291a4f-24cf-46ec-a109-ea2b2d41537f" />

Configured Lab-IT as a security group with assigned membership. Added a description identifying its purpose and selected one member for the group.

### 14. Create the HR Security Group

<img width="1857" height="913" alt="14" src="https://github.com/user-attachments/assets/152977fb-f715-4020-8850-89a9b4b14adf" />

Configured Lab-HR as a security group with assigned membership. Added a description identifying its purpose and selected one member for the group.

### 15. Create the Sales Security Group

<img width="1859" height="918" alt="15" src="https://github.com/user-attachments/assets/72c9c2c3-974d-4e6d-a4b6-7fd8512cc168" />

Configured Lab-Sales as a security group with assigned membership. Added a description identifying its purpose and selected one member for the group.

### 16. Verify the Departmental Security Groups

<img width="1850" height="924" alt="16" src="https://github.com/user-attachments/assets/1b139159-0e7d-4682-beeb-7e3687d80d39" />

Confirmed that Lab-IT, Lab-HR, and Lab-Sales appeared in the tenant as security groups with assigned membership.

### 17. Verify IT Group Membership

<img width="1853" height="906" alt="17" src="https://github.com/user-attachments/assets/4a939e5f-f271-4ec1-8d26-c1d7481c9948" />

Confirmed that ITSupport1 was a direct member of Lab-IT, matching the user’s department.

### 18. Verify HR Group Membership

<img width="1868" height="897" alt="18" src="https://github.com/user-attachments/assets/49aca9dc-742c-4274-b7a8-dcf97c32d633" />

Confirmed that HRUser1 was a direct member of Lab-HR, matching the user’s department.

### 19. Verify Sales Group Membership

<img width="1854" height="909" alt="19" src="https://github.com/user-attachments/assets/f713004b-1b31-4c21-b734-3af309d48123" />

Confirmed that SalesUser1 was a direct member of Lab-Sales, matching the user’s department.

### 20. Change ITSupport1’s Temporary Password

<img width="1846" height="922" alt="20" src="https://github.com/user-attachments/assets/e16b3a38-17a7-4d41-99ad-124a6f674bc6" />

Signed in as ITSupport1 and received the required password-change prompt. Replaced the temporary password with a new password before continuing.

### 21. Verify ITSupport1 Sign-In

<img width="1875" height="954" alt="21" src="https://github.com/user-attachments/assets/f4cca4eb-166a-49a9-b5fd-112d8f42703b" />

Successfully accessed the My Account page as ITSupport1 after changing the temporary password. The page displayed the expected username and IT Support Technician job title.

### 22. Change HRUser1’s Temporary Password

<img width="1567" height="814" alt="22" src="https://github.com/user-attachments/assets/f006adad-09cd-4605-81ae-4507f4bdfcde" />

Signed in as HRUser1 and received the required password-change prompt. Replaced the temporary password with a new password before continuing.

### 23. Verify HRUser1 Sign-In

<img width="1873" height="944" alt="23" src="https://github.com/user-attachments/assets/e1ca74e5-23ec-4246-b91c-9fdf3d93d74d" />

Successfully accessed the My Account page as HRUser1 after changing the temporary password. The page displayed the expected username and HR Assistant job title.

### 24. Change SalesUser1’s Temporary Password

<img width="1647" height="796" alt="24" src="https://github.com/user-attachments/assets/019f6918-959e-4db2-94e5-0d36ed84d34f" />

Signed in as SalesUser1 and received the required password-change prompt. Replaced the temporary password with a new password before continuing.

### 25. Verify SalesUser1 Sign-In

<img width="1860" height="923" alt="25" src="https://github.com/user-attachments/assets/47b6ffd1-c800-4e95-beb3-c7faa27dec20" />

Successfully accessed the My Account page as SalesUser1 after changing the temporary password. The page displayed the expected username and Sales Representative job title.

## Skills Demonstrated

- Microsoft Entra ID user provisioning
- User profile and department configuration
- Security group creation
- Assigned group membership management
- License and subscription review
- First-sign-in testing
- Temporary password replacement
- Technical documentation

## Part 1 Summary

Part 1 established a cloud identity lab with three departmental test users and three security groups. Each user’s group membership was verified, and all three accounts successfully completed their first sign-in and required password change.

This environment provides the foundation for configuring and testing MFA and sign-in protections in Part 2.

## Part 2: MFA Registration and Sign-in Log Review

### Overview

In this part of the lab, I verified that Security Defaults were enabled, registered Microsoft Authenticator for the ITSupport1, HRUser1, and SalesUser1 test accounts, and reviewed their sign-in activity in Microsoft Entra ID.

I confirmed each account’s registered authentication method and examined sign-in details to distinguish successful password authentication, MFA registration requirements, and normal sign-in interruptions.

### Technologies Used

- Microsoft Entra admin center
- Microsoft Entra ID Security Defaults
- Microsoft Authenticator
- My Sign-ins Security info portal
- Microsoft Entra ID sign-in logs

### 1. Verify Security Defaults

<img width="1913" height="910" alt="1" src="https://github.com/user-attachments/assets/2e6f06d7-362d-4b9f-900b-bf8c9dbfacae" />

Verified that Security Defaults were already enabled for the lab tenant. This established the identity security baseline used during this part of the project.

### 2. Begin Authenticator Registration for ITSupport1

<img width="1479" height="798" alt="2" src="https://github.com/user-attachments/assets/1e0d4c99-f69f-40c8-adc4-be44dc4d0106" />

Signed in as ITSupport1 and received a prompt to set up Microsoft Authenticator as an additional way to verify the account’s identity.

### 3. Complete Authenticator Registration for ITSupport1

<img width="772" height="679" alt="3" src="https://github.com/user-attachments/assets/8ea58165-7078-43a3-8689-81b4c58b42f5" />

Completed the registration process and received confirmation that Microsoft Authenticator had been added as the account’s default sign-in method.

### 4. Verify ITSupport1’s Registered Authentication Method

<img width="1915" height="988" alt="4" src="https://github.com/user-attachments/assets/de6e98c9-421f-47f4-bd47-1373eb91a912" />

Reviewed ITSupport1’s Security info page and confirmed that Microsoft Authenticator was listed for push multifactor authentication on an iPhone.

### 5. Begin Authenticator Registration for HRUser1

<img width="1189" height="717" alt="5" src="https://github.com/user-attachments/assets/3a72c1b4-e9c8-42d7-9aac-30116013af4a" />

Signed in as HRUser1 and received the account security prompt to register Microsoft Authenticator.

### 6. Complete Authenticator Registration for HRUser1

<img width="993" height="647" alt="6" src="https://github.com/user-attachments/assets/da34e88f-7bd1-4c28-bb57-555a4ff460cb" />

Completed Microsoft Authenticator registration for HRUser1 and received confirmation that it had been added as the default sign-in method.

### 7. Verify HRUser1’s Registered Authentication Method

<img width="1912" height="947" alt="7" src="https://github.com/user-attachments/assets/c6b6a426-3ece-4e8a-b96a-23b802e7c229" />

Reviewed HRUser1’s Security info page and confirmed that Microsoft Authenticator was registered for push multifactor authentication on an iPhone.

### 8. Begin Authenticator Registration for SalesUser1

<img width="1032" height="612" alt="8" src="https://github.com/user-attachments/assets/c5270645-6d77-453b-90fa-c64f25ec33a1" />

Signed in as SalesUser1 and began the Microsoft Authenticator registration process through the account security prompt.

### 9. Complete Authenticator Registration for SalesUser1

<img width="1017" height="650" alt="9" src="https://github.com/user-attachments/assets/d01c7e22-218e-4f85-b779-4ca2b38effd0" />

Received confirmation that Microsoft Authenticator had been added to SalesUser1 and set as the default sign-in method.

### 10. Verify SalesUser1’s Registered Authentication Method

<img width="1909" height="752" alt="10" src="https://github.com/user-attachments/assets/43b1739a-514a-4d42-a3af-08dde2b28752" />

Reviewed SalesUser1’s Security info page and confirmed that Microsoft Authenticator was listed for push multifactor authentication on an iPhone.

### 11. Review ITSupport1’s Sign-in Event

<img width="1903" height="920" alt="11" src="https://github.com/user-attachments/assets/d1636a07-442c-4776-a2ea-4c7713127698" />

Reviewed the Basic info tab for ITSupport1’s October 13 sign-in event. The event showed a successful sign-in with a single-factor authentication requirement.

### 12. Examine ITSupport1’s Authentication Details

<img width="1903" height="803" alt="12" src="https://github.com/user-attachments/assets/8822c492-72e0-4902-ac62-d488a2a7eb8e" />

The Authentication Details tab showed that password authentication succeeded using “Password in the cloud,” with the result “Correct password.” This event documented successful password authentication; it did not show a separate Microsoft Authenticator approval.

### 13. Review HRUser1’s Interrupted Sign-in

<img width="1914" height="902" alt="13" src="https://github.com/user-attachments/assets/77992f7e-0b95-4dcd-a4e0-f1ae0bc97198" />

Reviewed an HRUser1 sign-in event with a multifactor authentication requirement and an Interrupted status. The additional details stated that the user was presented with options to provide contact information for MFA.

### 14. Examine HRUser1’s Authentication Details

<img width="1898" height="871" alt="14" src="https://github.com/user-attachments/assets/de6e5060-7141-4c0e-a136-69d8e8c5ccd8" />

Confirmed that Security Defaults applied to this event. The password authentication step succeeded, while a subsequent step indicated that MFA was required and was not completed within this event. This documented an MFA registration interruption rather than a completed MFA sign-in.

### 15. Review SalesUser1’s Interrupted Sign-in

<img width="1903" height="903" alt="15" src="https://github.com/user-attachments/assets/48c2009e-ebe9-43df-b060-96a9692a846c" />

Reviewed SalesUser1’s sign-in event and its Interrupted status. The additional details identified the interruption as an expected part of the login flow in which the user is asked whether to remain signed in to the browser.

### 16. Examine SalesUser1’s Authentication Details

<img width="1908" height="767" alt="16" src="https://github.com/user-attachments/assets/9ef7e58a-1002-4d20-8426-3bfd9d4841ac" />

Verified that SalesUser1’s password authentication succeeded, with the result “Correct password.” Combined with the Basic info details, this showed that the interruption was associated with the “Stay signed in?” prompt. This event did not show a separate Microsoft Authenticator approval.

### Skills Demonstrated

- Reviewing tenant security settings
- Registering Microsoft Authenticator for multiple users
- Verifying registered authentication methods
- Reviewing user sign-in logs
- Interpreting authentication requirements and individual step results
- Investigating interrupted sign-in events
- Documenting findings based on the available evidence

### Summary

Registered Microsoft Authenticator for all three test accounts and confirmed push MFA registration through their Security info pages.

The sign-in log review demonstrated the importance of examining individual authentication steps and additional details. The selected events showed successful password authentication, an MFA registration requirement, and an expected interruption for the “Stay signed in?” prompt.

These findings distinguish successful authentication-method registration from evidence that MFA was completed during a specific sign-in.

## Part 3: Windows Endpoint Security Hardening

### Overview

In Part 3, I hardened a Windows 10 Pro virtual machine by strengthening password requirements, separating standard and administrator accounts, reviewing endpoint protection, and enabling security logging.

### Tools Used

VirtualBox, Windows 10 Pro, Local Users and Groups, Local Security Policy, Microsoft Defender Antivirus, Windows Defender Firewall, Command Prompt, and Event Viewer.

### 1. Creating a Standard Local Account

I created **LabUser1**, with the display name **Lab Standard User**, for security testing without administrator privileges.

<img width="1021" height="772" alt="1" src="https://github.com/user-attachments/assets/3a554425-ef2f-45a9-a646-d16f7b2f6c04" />

### 2. Verifying Standard-User Group Membership

I confirmed that LabUser1 belonged to the local **Users** group.

<img width="1025" height="785" alt="2" src="https://github.com/user-attachments/assets/de5ed992-ec0e-4649-b89e-42e5d66248f8" />

### 3. Reviewing the Original Password Policy

I reviewed the original password policy, which had a minimum password length of **0 characters** and complexity requirements disabled.

<img width="1022" height="772" alt="3" src="https://github.com/user-attachments/assets/a01a4507-f7b4-4f67-a439-ffbe55c72bbc" />

### 4. Setting the Minimum Password Length

I increased the minimum password length to **14 characters**.

<img width="1021" height="771" alt="4" src="https://github.com/user-attachments/assets/75eeeffa-a7be-4e0a-a3a7-4b768cbe04aa" />

### 5. Enabling Password Complexity

I enabled **Password must meet complexity requirements** in Local Security Policy.

<img width="1019" height="774" alt="5" src="https://github.com/user-attachments/assets/503f56dc-067c-4b58-85eb-cadd182c1304" />

### 6. Verifying the Updated Password Policy

I confirmed that the minimum password length was **14 characters** and password complexity was **Enabled**.

<img width="1020" height="774" alt="6" src="https://github.com/user-attachments/assets/6d6d8ea7-66f7-4605-8f36-d01d58043698" />

### 7. Reviewing Account Lockout Settings

I verified the existing threshold of **10 invalid logon attempts**, a **10-minute lockout duration**, and a **10-minute reset period**.

<img width="1021" height="777" alt="7" src="https://github.com/user-attachments/assets/9347f2aa-4731-493a-9677-12486fb2a3f3" />

### 8. Resetting the Standard Account Password

I reset LabUser1’s password to meet the strengthened requirements and received confirmation that the password had been set.

<img width="1030" height="775" alt="8" src="https://github.com/user-attachments/assets/d90d8e97-cc41-4f9d-9c4d-7429efd15862" />

### 9. Signing Out of the Administrator Session

I signed out to switch from the administrator account to the standard account for testing.

<img width="1029" height="773" alt="9" src="https://github.com/user-attachments/assets/7f31316a-a396-47c2-a96c-b5d9f62e6ab2" />

### 10. Signing In as the Standard User

I selected **Lab Standard User**, the display name for LabUser1, and signed in with its updated password.

<img width="1023" height="769" alt="10" src="https://github.com/user-attachments/assets/166a290f-7112-4175-8d38-366a6416bed3" />

### 11. Verifying Account Identity and Administrator Membership

I used `whoami` and `net localgroup Administrators` to confirm that I was signed in as **LabUser1** and that it was not a member of the Administrators group.

<img width="1024" height="764" alt="11" src="https://github.com/user-attachments/assets/805f0816-7a25-4839-aeb9-31d5a74ebc3d" />

### 12. Testing Administrative Elevation

I attempted to open an elevated Command Prompt from the standard account and verified that Windows requested separate administrator credentials.

<img width="1021" height="769" alt="12" src="https://github.com/user-attachments/assets/f2cb45bf-fc16-4736-8bbd-8f14cc35b094" />

### 13. Reviewing Microsoft Defender

I returned to the administrator account and opened Microsoft Defender, which initially showed no current threats and no available previous scan result.

<img width="1020" height="775" alt="13" src="https://github.com/user-attachments/assets/24cd3e00-0a82-4137-ad9c-8da3309dd556" />

### 14. Verifying Real-Time and Cloud Protection

I confirmed that Microsoft Defender’s **Real-time protection** and **Cloud-delivered protection** were enabled.

<img width="1022" height="765" alt="14" src="https://github.com/user-attachments/assets/7eb020a3-32ec-4020-90ff-6b420f13f4c8" />

### 15. Verifying Sample Submission and Tamper Protection

I confirmed that **Automatic sample submission** and **Tamper Protection** were enabled.

<img width="1027" height="772" alt="15" src="https://github.com/user-attachments/assets/0e79d03d-368c-49ff-9aad-b1185f7041ea" />

### 16. Accessing Protected Security Settings

I approved the Windows Security elevation prompt to access Microsoft Defender’s exclusion settings.

<img width="1035" height="764" alt="16" src="https://github.com/user-attachments/assets/40dd3cf1-10a6-4510-a34c-bf932f241d34" />

### 17. Reviewing Antivirus Exclusions

I checked Microsoft Defender’s Exclusions page and confirmed that no exclusions were listed.

<img width="1019" height="762" alt="17" src="https://github.com/user-attachments/assets/6d0cff16-c878-49c4-a993-d33599e00ed9" />

### 18. Checking for Security Intelligence Updates

I initiated a security intelligence update check; this image shows the check in progress rather than confirmation of an installed update.

<img width="1024" height="772" alt="18" src="https://github.com/user-attachments/assets/53a6ea7d-ea03-4a7d-acc0-5b600fc6bdf7" />

### 19. Reviewing Quick Scan Results

I completed a quick scan that checked **29,206 files** in **28 seconds** and reported **0 threats found**.

<img width="1026" height="774" alt="19" src="https://github.com/user-attachments/assets/f07c0c78-cfbb-4da9-ad3c-6c49be28f1a7" />

### 20. Verifying Firewall Protection

I confirmed that Windows Defender Firewall was enabled for the **Domain**, **Private**, and **Public** profiles, with Public shown as active.

<img width="1020" height="774" alt="20" src="https://github.com/user-attachments/assets/26e454ec-bec6-40cf-a4f4-06450c3e6db9" />

### 21. Reviewing Firewall Connection Defaults

I verified that all profiles blocked unmatched inbound connections and allowed unmatched outbound connections.

<img width="1025" height="773" alt="21" src="https://github.com/user-attachments/assets/fdc6352c-3a61-4cf5-9810-f7593a4bd7d0" />

### 22. Enabling Dropped-Packet Logging

I enabled **Log dropped packets** for the Public firewall profile while leaving successful-connection logging disabled and the log size limit at **4,096 KB**.

<img width="1022" height="773" alt="22" src="https://github.com/user-attachments/assets/3e12cc49-4386-4fd4-a496-746ab789a6d3" />

### 23. Enabling Logon Auditing

I configured **Audit Logon** to record both successful and failed logon attempts.

<img width="1019" height="777" alt="23" src="https://github.com/user-attachments/assets/14040c2a-5672-4be8-9bbf-e6b38860e16c" />

### 24. Verifying the Effective Audit Policy

I ran `auditpol /get /subcategory:"Logon"` and confirmed that the effective setting was **Success and Failure**.

<img width="1020" height="775" alt="24" src="https://github.com/user-attachments/assets/285b3eff-3fb5-49c0-8dcc-8780f8ed48bd" />

### 25. Filtering Security Events

I configured an Event Viewer Security log filter for **4624**, successful logons, and **4625**, failed logons.

<img width="1028" height="775" alt="25" src="https://github.com/user-attachments/assets/667898ec-39da-49f7-9f63-661088f69bbe" />

### 26. Reviewing a Failed Logon

I examined **Event ID 4625** for LabUser1 at **9:08:06 PM**, which recorded a failed interactive logon with **Logon Type 2**.

<img width="1016" height="775" alt="26" src="https://github.com/user-attachments/assets/d4b7f985-f5bc-4cf4-96d1-1ed5c48f5516" />

### 27. Reviewing a Successful Logon

I examined **Event ID 4624** for LabUser1 at **9:07:12 PM**, documenting a separate successful logon that occurred before the failed event above.

<img width="1014" height="768" alt="27" src="https://github.com/user-attachments/assets/625ecaa2-dff8-4e42-be7c-a04508d8d385" />

### Skills Demonstrated

- Local user and group administration
- Standard-user and administrator separation
- Password policy configuration
- Account lockout policy review
- User Account Control testing
- Microsoft Defender review and scanning
- Firewall configuration and logging
- Logon auditing and Security event analysis

### Summary

In this part, I strengthened local password requirements, tested standard-user restrictions, reviewed Microsoft Defender and firewall protection, enabled dropped-packet logging for the Public profile, and verified successful and failed logon auditing.

The virtual machine remained a standalone Windows 10 lab endpoint during Part 3. The work demonstrates the specific controls configured and verified, rather than a complete security assessment or confirmation that Windows was fully patched.
