## 📧 Automation of Distribution List (DL) Assignment for New Joiners & Transfers 🚀

### Streamlining User Access Management & Enhancing Onboarding Efficiency 🧑‍🤝‍🧑 - Saving **4-5 Man-Hours Daily!**

This project automated the manual and time-consuming process of assigning and updating Distribution List (DL) memberships for new employees and employees undergoing department transfers at YES Bank. The solution streamlines user access management, saves **4-5 man-hours daily**, enhances onboarding efficiency, and ensures timely and accurate DL assignments, eliminating manual errors and delays.

### 🎯 Requirement: Manual, Time-Consuming, and Inefficient DL Management

The existing process for DL assignment and updates presented several challenges:

*   **😓 Manual YESIT Portal Process:**  Adding or removing employees from DLs required manual navigation through the YESIT portal, involving multiple steps and manual data entry.
*   **⏱️ Time-Consuming Request Process:**  Submitting DL update requests through the portal, tracking approvals, and following up with approvers was a time-consuming process, especially for onboarding new joiners who needed access quickly.
*   **⏳ Delays in Access Provisioning:**  Manual request processes caused delays in providing new employees with necessary DL access, hindering their productivity during the initial onboarding phase.
*   **⚠️ Risk of Errors & Omissions:** Manual DL management was prone to errors, inconsistencies, and the risk of missing new joiners or failing to update DLs for employee transfers.
*   **📉 Inefficient Onboarding Experience:**  New employees faced a cumbersome and confusing access request process, impacting their onboarding experience and initial productivity.
*   **🧑‍🤝‍🧑 Heavy Reliance on User Intervention:** The entire process was heavily reliant on manual user actions and follow-ups from both employees and IT support.

### 🤖 Automation Approach:  Intelligent, Data-Driven, and End-to-End DL Management

Our automation strategy focused on creating a fully automated and intelligent DL assignment system:

*   **🔄 Automated New Joiner Detection from HRIS DB:** 🤖 Bot automatically connects to the **HRIS (Human Resources Information System) database (MSSql DB)** daily to fetch a list of **newly joined employees**.
*   **💼 Data-Driven DL Assignment Logic:** 🤖 Bot utilizes a **predefined mapping (maintained in MMA - Master Maintenance Application)** to determine appropriate DL assignments based on employee attributes: **Business Unit Name, Location Code, Gender, and Designation Code**. This mapping is dynamically fetched via a **REST API request to MMA**.
*   **➕ Automated DL Addition using PowerShell:** 🤖 Based on the mapping, the bot automatically adds new employees to their respective DLs using **PowerShell commands**, directly managing DL memberships.
*   **🔄 Automated Transfer Handling:** 🤖 Bot also detects **employee transfers** by comparing daily HRIS data with previous data. For transferred employees:
    *   **Removes from Old DLs:** 🤖 Bot automatically removes the employee from their **previous DL memberships** using PowerShell commands.
    *   **Adds to New DLs:** 🤖 Bot automatically adds the transferred employee to their **new DL memberships** based on their updated department/role, again using PowerShell commands and the MMA mapping.
*   **💾 IT Team DB Update (Oracle DB):** 🤖 For record-keeping and IT audit purposes, the bot updates an **IT team's database (Oracle DB)** with details of all DL additions and removals performed, providing a centralized log for IT maintenance and tracking.
*   **📊 Automated Reporting & Email Notifications:** 🤖 After each execution, the bot generates a **detailed Excel report** summarizing all DL additions and removals performed. This report is automatically **emailed to relevant stakeholders**, providing transparency and confirmation of DL updates.

### ✨ Role of Automation:  Transforming DL Management from Manual Burden to Automated Efficiency

Automation fundamentally transformed DL management from a manual, error-prone process into a streamlined, efficient, and hands-off system:

*   **End-to-End Automation:** 🤖 Bot automates the entire DL assignment and update lifecycle, from new joiner detection to reporting, eliminating manual intervention.
*   **Proactive and Timely Access Provisioning:** 🚀 New employees automatically gain access to relevant DLs from day one, significantly improving onboarding efficiency and time-to-productivity.
*   **Dynamic and Accurate DL Updates:** 🔄 Bot dynamically manages DL memberships based on real-time HR data and defined business rules, ensuring accurate and up-to-date DL assignments.
*   **Reduced IT Support Workload:** 🧑‍🤝‍🧑 Automation drastically reduces the workload on IT support teams by eliminating manual request processing and approval tracking for DL updates.
*   **Hassle-Free Onboarding Experience:** 🎉 New joiners experience a seamless onboarding process without needing to navigate complex access request procedures, improving their initial impression and engagement.
*   **Improved Scalability & Accuracy:** 📈 Automated system is highly scalable to handle growing employee numbers and ensures consistent, error-free DL management, eliminating manual inconsistencies.

### 🚀 Benefits Achieved:  Streamlined Onboarding, Time Savings, and Enhanced User Management

The Automation of DL Assignment project delivered significant benefits:

*   **⏱️ 4-5 Man-Hours Saved Daily:** Automation saves approximately **4-5 man-hours daily** by eliminating manual DL management tasks, freeing up valuable IT and HR resources.
*   **🚀 Streamlined New Employee Onboarding:** New joiners gain immediate access to necessary DLs, significantly streamlining the onboarding process and improving their initial experience.
*   **✅ Enhanced Accuracy & Reduced Errors:** Automated DL assignment eliminates manual errors, ensuring accurate and consistent DL memberships across the organization.
*   **🧑‍🤝‍🧑 Reduced IT Support Burden:** IT teams experience a significant reduction in workload related to DL management requests, freeing up their time for more strategic IT initiatives.
*   **🎯 Improved Operational Efficiency:** Automation streamlines user access management, improving overall operational efficiency within IT and HR departments.
*   **🛡️ Enhanced Security & Compliance:** Automated and centrally managed DL assignments improve security and compliance by ensuring appropriate access control and reducing the risk of unauthorized access.

### 🛠️ Technologies Used:

*   **RPA Tool:** Process Studio (AutomationEdge)
*   **Database:** HRIS DB (MSSql DB), IT Team DB (Oracle DB)
*   **API Integration:** REST API (MMA - Master Maintenance Application)
*   **Scripting:** PowerShell (for Active Directory/Exchange Management - DL manipulation)
*   **Automation Types:** Database Integration, API Integration, Scripting Automation, Scheduled Automation, Email Automation, Excel Reporting.

### 🎉 Conclusion:  Revolutionizing User Access Management with Intelligent Automation -  Seamless Onboarding and Efficient DL Management!

The Automation of DL Assignment project represents a significant advancement in user access management at YES Bank. By automating a previously manual, time-consuming, and error-prone process, the solution delivers substantial time savings, enhances onboarding efficiency, improves data accuracy, and streamlines IT operations. This intelligent automation exemplifies the power of RPA to transform core IT processes, enhance user experience, and drive operational excellence in user access management and onboarding workflows.
