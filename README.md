# Importing & Securing Data in ServiceNow

---

### 📌 Project Overview
This project demonstrates how to import employee training data into ServiceNow, link it with employee records, and enforce secure access using ACLs and role-based permissions. It highlights best practices for data integrity and access control within an enterprise ServiceNow environment.

---

### ✨ Key Features

* **Data Import & Mapping:** Import structured data from external files using `Import Sets` & `Transform Maps`.
* **Dot-Walking:** Automatically retrieve related employee information (like Department) from linked records.
* **Access Control (ACLs):** Restrict access at the table and field level based on user roles.
* **Role-Based Permissions:** Provide separate and distinct access rights for `HR Manager` and `Admin` users.
* **Custom Tables & Fields:** Create tailored data structures to manage employee training records efficiently.
* **Impersonation Testing:** Verify visibility and edit permissions for different user roles to ensure security policies are correctly enforced.
* **Scalability & Security:** Designed with a framework that handles large datasets while maintaining robust security operations.

---

### 🛠️ Tech Stack

* **Platform:** ServiceNow
* **Modules Used:**
    * Import Sets
    * Transform Maps
    * Access Control Lists (ACLs)
    * Roles & Permissions
    * System Security
* **Tools:**
    * ServiceNow Studio
    * ACL Editor

---

### 📂 Project Workflow

1.  **Ideation:** Define the core problem and the scope of the project.
2.  **Requirement Analysis:** Specify the need for a custom table, import sets, role definitions, and specific ACLs.
3.  **Design:** Architect the custom `Employee Training` table with the following fields: `Training Name`, `Completion Date`, `Status`, and an `Employee` field referencing the User `[sys_user]` table.
4.  **Development:**
    * Import the external data using Import Sets and configure Transform Maps.
    * Configure dot-walking to display the employee's department directly in the training record list.
    * Implement ACLs to manage Read/Write security rules.
    * Create a dedicated `HR Manager` role and assign the necessary permissions.
5.  **Testing:**
    * Impersonate the `HR Manager` to verify appropriate access to view and modify training records.
    * Impersonate other users (without the specific role) to verify that access is correctly restricted.
6.  **Conclusion:** Evaluate the overall success of the secure data import process and the effectiveness of the access management solution.
