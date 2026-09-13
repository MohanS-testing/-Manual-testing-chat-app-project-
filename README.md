# -Manual-testing-chat-app-project-Manual QA Testing Project

## 📌 Project Overview
- **Project Name:** Friend's Mobile Chat Application (VIP-based Chatonic App)
- **Tested By:** Mohan Srivastav
- **Testing Type:** Manual Functional, UI, Performance & Billing Testing
- **Tools Used:** Microsoft Excel, Jira for Defect Tracking

---

## 📄 Test Artifacts Included
- 📋 **[Test Scenarios](./Test_Scenarios.xlsx)** – High-level scenarios covering core app modules.
- 🧪 **[Test Cases](./Test_Cases.xlsx)** – Detailed test execution steps, data, and retest results.
- 🐞 **[Bug Report](./Bug_Report.xlsx)** – Comprehensive defect logs with steps to reproduce and severity levels.
- 📊 **[Test Result Summary](./Test_Result_Summary.xlsx)** – Final execution metrics and overall status.

---

## 🐞 Bugs Summary & Status

| Bug ID | Module | Issue Description | Severity | Status | Retest Verdict |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **BUG-001** | Login/Authentication | Application logs in successfully using email address instead of username | Medium | Fixed | Pass - Verified |
| **BUG-002** | Room Chat/Messaging | Messages delayed when room had ~40 active participants | High | Fixed | Pass - Verified |
| **BUG-003** | Room Chat/UI | Message input box floated higher with noticeable gap when keyboard opened | Medium | Fixed | Pass - Verified |
| **BUG-004** | Mode VIP Subscription/Billing | VIP purchase failed with Google Play Error Code 3 (Billing Unavailable) | Critical | Fixed | Pass - Verified |

---

## 📊 Test Execution Metrics
- **Total Test Scenarios:** 4
- **Total Test Cases Executed:** 5
- **Total Bugs Found:** 4
- **Bugs Fixed & Verified:** 4
- **Open Bugs:** 0
- **Overall Test Result:** **PASS** (All identified defects fixed and verified)
