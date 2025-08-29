# Importing-Securing-Data-in-ServiceNow
📌 Project Overview

This project demonstrates how to import employee training data into ServiceNow, link it with employee records, and enforce secure access using ACLs and role-based permissions. It highlights best practices for data integrity and access control within an enterprise ServiceNow environment.

✨ Key Features

Data Import & Mapping – Import structured data from external files using Import Sets & Transform Maps.

Dot-Walking – Automatically retrieve related employee information (like Department) from linked records.

Access Control (ACLs) – Restrict access at table/field level based on roles.

Role-Based Permissions – Provide separate access rights for HR Manager and Admin users.

Custom Tables & Fields – Create tailored structures to manage employee training records.

Impersonation Testing – Verify visibility and editability for different user roles.

Scalability & Security – Designed to handle large datasets while ensuring secure operations.



🛠️ Tech Stack

Platform: ServiceNow
Modules Used: Import Sets, Transform Maps, ACLs, Roles, System Security
Tools: ServiceNow Studio, ACL Editor



📂 Project Workflow

Ideation – Define problem and scope.

Requirement Analysis – Custom table, import sets, ACLs, role definitions.

Design – Employee training table with fields: Training Name, Completion Date, Status, Employee (reference to sys_user).

Development –
Import data via Import Sets & Transform Maps
Configure dot-walking for employee department
Implement ACLs for Read/Write security
Create HR Manager role and assign permissions

Testing –
Impersonate HR Manager → verify access to training records
Impersonate other users → verify restricted access

Conclusion – Evaluate success of secure data import and access management.
