# 📱 Mobile Application Manual Testing & QA Portfolio

![Platform](https://img.shields.io/badge/Platform-Android%2014-blue)
![RAM](https://img.shields.io/badge/RAM-6%20GB-purple)
![Network](https://img.shields.io/badge/Network-Wi--Fi%20%2F%204G-orange)
![Test Status](https://img.shields.io/badge/Testing-Completed-brightgreen)
![Pass Rate](https://img.shields.io/badge/Pass%20Rate-40.0%25-red)

## 📌 Project Overview
This repository contains a full **Software Testing Life Cycle (STLC)** manual QA testing project for an Android-based chat/social mobile application featuring real-time messaging and **VIP In-App Purchases (Google Play Billing)**.

The testing cycle covered core functional flows, user experience, credential/session security (including brute-force vulnerability testing), real-time sync performance, network resilience, and monetization mechanisms to evaluate release readiness.

---

## ⚙️ Test Scope & Hardware Environment

* **Target Platform:** Android (Android 14)
* **Hardware Specs:** Android Smartphone (6 GB RAM)
* **Network Conditions:** Wi-Fi & 4G LTE (including throttled weak-network simulation)
* **Testing Type:** Manual Black-Box Functional & Security Testing
* **Tester:** Mohan Srivastav
* **Modules Covered:**
  * Authentication & Brute-Force Rate Limiting Security
  * Session Management & Multi-Device Security
  * Real-Time Messaging & Room Capacity Performance
  * Media Uploads & Profile Management
  * Runtime Permissions & System Notifications
  * Network Resilience & Offline Modes
  * VIP In-App Monetization (Google Play Billing)
  * UI Layout, Themes, & Screen Orientation / Auto-Rotation

---

## 📊 Test Execution Summary

| Metric | Details |
| :--- | :--- |
| **Total Scenarios Executed** | **15 Scenarios** (SC-01 to SC-15) |
| **Total Test Cases Executed** | **30 Test Cases** (TC-001 to TC-030) |
| **Passed Test Cases** | **12** (40.0%) |
| **Failed Test Cases** | **18** (60.0%) |
| **Total Defects Identified** | **18 Defects** |
| **Defect Severities** | **6 Critical** \| **6 High** \| **6 Medium** |

---

## 🔴 Critical Defects & Security Vulnerabilities

Out of 18 defects identified, 6 critical issues severely impact application security, retention, and monetization:

1. **VIP Billing Failure:** Google Play Billing verification error blocks in-app purchases (`TC-024` / `BUG-024`).
2. **Session Drop on App Backgrounding:** App force-invalidates user login session upon backgrounding (`TC-007` / `BUG-007`, `TC-018` / `BUG-018`).
3. **Session Loss on Transient Drops:** Brief network drops force immediate user logout instead of auto-reconnecting (`TC-021` / `BUG-021`).
4. **UI Freeze on Weak Connection:** Application freezes (ANR-like state) without loading indicators on slow networks (`TC-022` / `BUG-022`).
5. **Brute-Force Rate Limiting Gap:** Unlimited password attempts allowed on login screen without lockout or CAPTCHA protection (`TC-005` / `BUG-005`).
6. **No Screen Rotation Support:** Application UI remains permanently locked in Portrait mode even with OS Auto-Rotate enabled on Android 14 (`TC-030` / `BUG-030`).

---

## 📁 Repository Deliverables & Artifacts

The repository includes complete, industry-standard STLC documentation:

* 📄 **[Test Plan (Word Document)](./Test_Plan.docx):** Defines scope, strategy, exit criteria, entry criteria, hardware specs, and risks.
* 📄 **[Test Scenarios Sheet (Excel)](./Test_Scenarios_2.xlsx):** Feature-wise scenario breakdown with status roll-up.
* 📄 **[Test Cases Document (Excel)](./Test_Cases_2.xlsx):** 30 step-by-step test cases with expected results.
* 📄 **[Test Execution Record (Excel)](./Test_Execution_Record.xlsx):** Log of execution timestamps, test environments, and execution tracking.
* 📄 **[Test Result Log (Excel)](./Test_Result_Log.xlsx):** Pass/Fail results with actual vs. expected behavior mapping.
* 🐞 **[Defect Report Log (Excel)](./Defect_Report.xlsx):** Detailed bug reports with repro steps, severities, and priorities.
* 📊 **[Executive Test Summary Report (PDF)](./Test_Summary.pdf):** Formal summary outlining execution statistics, key findings, and recommendations.

---

## 💡 Key Recommendations for Development Team

1. **Fix Monetization & Security:** Resolve Google Play Billing verification errors and implement rate-limiting/lockout logic on login endpoints.
2. **Stabilize Session Persistence:** Fix background state loss and network reconnection handling to eliminate forced logouts.
3. **Enhance UI/UX Handling:** Implement auto-rotation support for Landscape mode on Android 14 and proper loading states for low-bandwidth states.

---

## 👤 Author & QA Tester

* **Name:** Mohan Srivastav
* **Role:** Manual QA Tester
* **Focus:** Mobile Testing, Security & Brute-Force Testing, STLC Documentation
