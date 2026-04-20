# 📄 Smart Leave Management System for Nigerian Organisations  
**Built with Microsoft Forms, Power Automate & Excel Online**  
*A step-by-step walkthrough of my Microsoft Elevate AI Developers Program Capstone Project*

---

## 🚀 Overview  

In many Nigerian organisations today, leave requests are still handled informally—through WhatsApp messages, phone calls, or verbal approvals. While this may seem convenient, it often leads to missing records, approval disputes, payroll inconsistencies, and lack of accountability.  

This project was built to solve that problem by transforming an unstructured process into a fully automated, digital workflow using Microsoft 365 tools. It introduces a structured, trackable, and auditable leave management system that ensures transparency from submission to final decision.  

Employees can submit requests digitally, managers can approve or reject in real time, and all actions are logged automatically—creating a reliable system for HR operations.

---

## 🚨 Problem Statement  

Many Nigerian workplaces rely on informal communication channels for leave approvals. This results in:

- ❌ No proper record of requests  
- ❌ Approval disputes between staff and management  
- ❌ Payroll and HR inconsistencies  
- ❌ Lack of audit trail  

There is a clear need for a structured and automated solution.

---

## 🎯 Project Goal  

The goal of this project is to:

- Digitize the leave request process  
- Automate approvals using workflow logic  
- Maintain a central audit log of all requests  
- Improve transparency and accountability in HR processes  

---

## 🛠 Tools & Technologies  

- **Microsoft Forms** – Data collection (Leave requests)  
- **Power Automate** – Workflow automation  
- **Excel Online (OneDrive)** – Data storage (Audit log)  
- **Microsoft Outlook** – Email notifications  
- **Microsoft Approvals** – Manager decision system  

---



---

## 📝 Step-by-Step Build Process  

### Step 1: Create Microsoft Form  

- Form Name: **Staff Leave Request Form**  
- Fields include:  
  - Employee Name  
  - Employee ID  
  - Department  
  - Leave Type  
  - Start Date  
  - End Date  
  - Number of Days  
  - Reason  
  - Cover Arranged  
  - Manager Email  

---

### Step 2: Prepare Excel Audit Log  

- File: `Leave_Requests_Log.xlsx`  
- Table Name: `Table2`  
- Key Column: **Staff ID**  

Columns include:  
- Employee Name  
- Employee Email  
- Staff ID  
- Department  
- Leave Type  
- Start Date  
- End Date  
- Days Requested  
- Reason  
- Manager Email  
- Cover Arranged  
- Approval Status  
- Manager Comments  
- Decision Date  

---

### Step 3: Build Power Automate Flow  

**Trigger:**  
- When a new response is submitted (Microsoft Forms)

**Key Actions:**  
1. Get response details  
2. Add row to Excel (Status = Pending)  
3. Send acknowledgement email  
4. Start approval process  
5. Condition check (Approve / Reject)  

---

### Step 4: Approval Logic  

- Approval Type: **Approve/Reject – First responder**  
- Condition:  




---

### Step 5: If Approved  

- ✅ Update Excel → Status = Approved  
- ✅ Save manager comments  
- ✅ Capture decision date  
- ✅ Send approval email  
- ✅ Create calendar event  

---

### Step 6: If Rejected  

- ❌ Update Excel → Status = Rejected  
- ❌ Save manager comments  
- ❌ Capture decision date  
- ❌ Send rejection email  

---

## 📧 Email Templates  

### Acknowledgement  

**Subject:** Your Leave Request Has Been Received  

Dear [Employee Name],  

Your leave request has been received and forwarded for approval.  

You will be notified once a decision is made.  

Regards,  
HR Team  

---

### Approved  

**Subject:** Leave Request Approved  

Dear [Employee Name],  

Your leave request has been approved.  

Please ensure proper handover before your leave begins.  

Regards,  
HR Team  

---

### Rejected  

**Subject:** Leave Request Not Approved  

Dear [Employee Name],  

Your leave request was not approved.  

Please contact your manager for further clarification.  

Regards,  
HR Team  

---

## 📊 Test Results  

| Employee | Leave Type | Status | Comment |
|----------|-----------|--------|---------|
| Abdul-Hakeem | Maternity | Approved | Approved successfully |
| Emeka | Sick Leave | Rejected | Medical report required |
| Fatima | Emergency | Pending | — |

---

## ⚠️ Limitations  

1. No leave balance validation  
2. No escalation if manager delays approval  
3. Limited to Microsoft 365 environment  

---

## 🔮 Future Improvements  

- Add leave balance validation (SharePoint integration)  
- Add approval reminders and escalation logic  
- Build Power BI dashboard for HR insights  
- Enable mobile-friendly interface  
- Add role-based access control  

---

## 💡 Key Takeaways  

- Automation improves HR efficiency  
- Structured workflows reduce errors  
- Audit logs enhance accountability  
- Low-code tools can solve real business problems  

---

## 🏁 Conclusion  

This project demonstrates how Microsoft Power Platform tools can transform everyday organisational processes into efficient, automated systems. By replacing informal communication with a structured workflow, organisations can improve transparency, reduce errors, and make better HR decisions.  

---

## 👋 About the Author  

Hi, I'm **Rofiah Abdul-Azeez**, an aspiring Data Analyst and Power Platform Developer passionate about building real-world automation solutions using low-code tools.  

I enjoy turning manual processes into efficient digital systems that create real impact.  

---

## 📌 Notes  

- This project was built using a Microsoft 365 Developer sandbox environment  
- External access may be restricted  
- Data used is for demonstration purposes only  

---
## ⚙️ System Architecture  
