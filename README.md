# TULA SETU – Digital Bridge to Verified Measurement

> A digital platform for modernizing the verification and certification process for weighing and measuring instruments.

## 📌 Overview

**TULA SETU** is a digital platform designed to modernize and streamline the verification and certification lifecycle of weighing and measuring instruments.

The platform addresses challenges such as paper-based records, scattered verification information, manual processing, certificate authentication, expiry tracking, and re-verification management.

It provides a proposed centralized workflow connecting **Instrument Owners, Administrators, Legal Metrology Officers (LMOs), and Government Approved Test Centres (GATCs).**

The current version is a **frontend prototype using sample/default data**, while the complete full-stack implementation is currently under development.

---

## 🎯 Problem Statement

The existing verification process can involve multiple stakeholders and several manual steps, making it difficult to:

* Maintain centralized instrument and verification records
* Track verification applications
* Manage inspection schedules
* Record field verification observations
* Track certificate validity and expiry
* Authenticate certificates conveniently
* Manage re-verification activities
* Reduce dependence on paper-based records

---

## 💡 Proposed Solution

TULA SETU proposes a centralized digital workflow:

```text
Instrument Registration
        ↓
Online Verification Application
        ↓
Admin Review & Assignment
        ↓
Inspection Scheduling
        ↓
Field Verification
        ↓
Observations + Photos
        ↓
Verification Result
        ↓
     ┌───────────────┐
     │     PASS?     │
     └───────┬───────┘
         YES │ NO
             │
             ↓
   Digital Certificate       Recheck / Re-inspection
       + QR Code
             ↓
   Validity & Expiry
      Monitoring
             ↓
      Re-verification
```

---

## ✨ Key Features

### 📝 Instrument Registration

* Register weighing and measuring instruments
* Maintain instrument information digitally

### 📋 Online Verification Applications

* Submit verification applications online
* Centralized application management

### 👨‍💼 Admin Dashboard

* Review applications
* Assign verification activities
* Manage schedules
* Monitor applications and certificates
* Track expiry information

### 🔍 Field Verification

LMOs/GATCs can:

* Access assigned inspection details
* Perform field verification
* Record observations
* Upload photographs
* Submit verification results

### 📜 Digital Certificates

* Generate digital verification certificates
* Maintain certificate records
* Track certificate validity

### 🔳 QR-Based Verification

* QR code associated with digital certificates
* Convenient certificate authentication
* Access verification details digitally

### 🔄 Recheck & Re-verification

* Support recheck/re-inspection workflows
* Track re-verification activities
* Monitor certificate validity and expiry

### ⏰ Expiry Monitoring

* Track certificate expiry
* Support automated expiry alerts
* Help reduce missed re-verification deadlines

> **Note:** These features represent the proposed system functionality. The current frontend prototype demonstrates these concepts using sample/default data, while complete functionality is being developed.

---

## 👥 Stakeholders

| Stakeholder                       | Role                                                                   |
| --------------------------------- | ---------------------------------------------------------------------- |
| **Instrument Owner / Business**   | Register instruments and submit verification applications              |
| **Administrator**                 | Review applications, manage assignments and schedules, monitor records |
| **Legal Metrology Officer (LMO)** | Perform field verification and submit inspection results               |
| **GATC**                          | Perform authorized testing and verification activities                 |

---

## 🏗️ System Architecture

```text
┌───────────────────────────────┐
│       Web Application         │
│   Instrument Owner / Admin    │
└───────────────┬───────────────┘
                │
                ↓
┌───────────────────────────────┐
│       FastAPI Backend          │
│   Application & Verification  │
│       Workflow Management      │
└───────────────┬───────────────┘
                │
                ↓
┌───────────────────────────────┐
│        MySQL Database          │
│ Instruments | Applications     │
│ Certificates | Verification    │
│ Records | Expiry Information  │
└───────────────────────────────┘

        ↑
        │
┌───────────────────────────────┐
│      Mobile Application       │
│       LMO / GATC Field        │
│         Verification           │
└───────────────────────────────┘
```

> The architecture represents the planned full-stack implementation. The current prototype primarily demonstrates the frontend.

---

## 🛠️ Technology Stack

### Frontend

* React.js

### Backend

* Python
* FastAPI
* REST API

### Database

* MySQL

### Other Technology

* QR Code Technology

---

## 🔄 Verification Lifecycle

TULA SETU follows a lifecycle-based approach:

**Register → Apply → Review → Schedule → Verify → Certify → Authenticate → Monitor → Re-verify**

The current prototype demonstrates the proposed workflow using sample/default data.

---

## 📊 Expected Impact

TULA SETU aims to provide:

* Reduced dependence on paper-based records
* Faster digital application and verification workflows
* Improved transparency of verification status
* Centralized verification records
* Convenient certificate authentication
* Better certificate expiry monitoring
* Structured field inspection records
* Improved administrative visibility
* Easier management of re-verification activities

---

## 🚀 Prototype

**Live Prototype:** [TULA SETU](https://tula-setu.netlify.app/)  

The current live prototype demonstrates the proposed frontend experience and workflow using sample/default data.

The full-stack implementation, including backend services, database integration, authentication, and complete end-to-end functionality, is currently under development.

---

## 📚 Research & References

The project is based on the relevant Legal Metrology framework and reference materials, including:

* Legal Metrology Act, 2009
* Legal Metrology (General) Rules, 2011
* Legal Metrology (Government Approved Test Centre) Rules, 2013
* Department of Consumer Affairs – Legal Metrology resources
* Other relevant Legal Metrology rules and guidelines

---

## 🏆 Project Context

**Project:** TULA SETU – Digital Bridge to Verified Measurement

**Domain:** Legal Metrology / Digital Verification

**Hackathon:** Smart India Hackathon (SIH)

---

## 🚧 Project Status

**Current Status:** Frontend Prototype

The current version demonstrates the proposed digital verification workflow and user interface using sample/default data.

The complete implementation is currently under development and will include backend services, database integration, authentication, persistent data management, and complete end-to-end workflows.

The project is being developed toward a fully functional digital verification and certification platform.

---

## 🔮 Future Development

The following components are planned as the project progresses:

1. FastAPI backend integration
2. MySQL database integration
3. Secure authentication and role-based authorization
4. Persistent instrument and application records
5. Real application processing
6. LMO/GATC verification workflow
7. Automated certificate generation
8. QR-based certificate validation
9. Automated expiry notifications
10. Complete frontend, backend, and database integration
