# SAP-ABAP-Final-Project

# 🏭 SAP ERP Implementation — NovaTex Industries Pvt. Ltd.

An end-to-end SAP S/4HANA ERP implementation project for a fictitious textile manufacturing company, covering core business processes across Finance, Procurement, and Sales.

📘 Academic Project | B.Tech CSE (SAP Data Analytics)  
👨‍💻 Author: Ayushmaan Sinha  

---

## 📖 Project Overview

NovaTex Industries Pvt. Ltd. is a mid-sized textile and apparel manufacturer facing operational inefficiencies due to fragmented legacy systems.

This project demonstrates the implementation of a fully integrated SAP ERP system to:

- Eliminate data silos  
- Enable real-time financial reporting  
- Streamline procurement and inventory  
- Automate sales and billing processes  
- Ensure GST compliance  

---

## 🚨 Problem Statement

The organization faced several key challenges:

-  Disconnected financial systems (no real-time reporting)  
-  Manual procurement via spreadsheets  
-  Inefficient sales order handling (email/phone-based)  
-  No integration between departments  
-  Compliance risks due to lack of audit trails  

---

## 💡 Solution

Implemented **SAP S/4HANA (On-Premise)** with three core modules:

| Module | Description |
|--------|------------|
| **FI (Financial Accounting)** | GL, AP, AR, GST configuration |
| **MM (Materials Management)** | Procurement & inventory (P2P cycle) |
| **SD (Sales & Distribution)** | Sales lifecycle (O2C cycle) |

✅ Real-time integration across all modules  
✅ Automated accounting entries  
✅ End-to-end business process coverage  

---

## 🧰 Tech Stack

- **ERP Platform:** SAP S/4HANA (2023)
- **Database:** SAP HANA (In-Memory)
- **Configuration:** SPRO (IMG)
- **Development:** ABAP
- **Reporting:** SAP Fiori Apps, Report Painter
- **Integration:** FI-MM, FI-SD, MM-SD

---

## 🏢 Company Blueprint

- **Industry:** Textile & Apparel  
- **Headquarters:** Surat, India  
- **Plants:** Surat, Ahmedabad, Pune  
- **Revenue:** ₹480 Cr (Fictitious)  
- **Employees:** ~1800  

### SAP Organizational Structure

- Company Code: `NTXL`  
- Plants: `NTX1`, `NTX2`, `NTX3`  
- Sales Org: `SO01`  
- Purchasing Org: `PO01`  
- Chart of Accounts: `NTCA`  

---

## 🔄 Core Business Processes

### 📥 Procure-to-Pay (P2P) — MM + FI

1. Purchase Requisition (ME51N)  
2. Purchase Order (ME21N)  
3. Goods Receipt (MIGO)  
4. Invoice Verification (MIRO)  
5. Payment Run (F110)  

💰 Automatic FI postings:
- Stock Dr → GR/IR Cr  
- GR/IR Dr → Vendor Cr  

---

### 📤 Order-to-Cash (O2C) — SD + FI

1. Sales Order (VA01)  
2. Delivery (VL01N)  
3. Post Goods Issue (VL02N)  
4. Billing (VF01)  
5. Payment Receipt (F-28)  

💰 Automatic FI postings:
- COGS Dr → Inventory Cr  
- AR Dr → Revenue + GST Cr  

---

## 🔗 Module Integration

### FI–MM Integration
- Goods Receipt → Auto accounting entry  
- Invoice → Vendor liability  
- Payment → Bank clearing  

### FI–SD Integration
- Billing → AR + Revenue posting  
- PGI → Inventory reduction  
- Payment → AR clearing  

### MM–SD Integration
- Real-time stock availability check  
- MRP triggered from sales demand  

---

## ✨ Key Highlights

- 🇮🇳 **GST-Compliant Tax Configuration** (CGST, SGST, IGST)  
- 🏭 **Multi-Plant Architecture** with centralized procurement  
- 🌍 **Domestic + Export Sales Channels**  
- ⚙️ **Automatic Account Determination (OBYC, VKOA)**  
- 🔄 Full **P2P and O2C with accounting impact tracking**  

---

## 📁 Project Structure
NovaTex-SAP-Project/
│
├── README.md
├── docs/
│ ├── Project_Report.pdf
│ ├── Blueprint.xlsx
│ └── IMG_Config_Steps.docx
│
├── screenshots/
│ ├── FI/
│ ├── MM/
│ └── SD/
│
├── config/
│ ├── gl_accounts.csv
│ ├── material_master.csv
│ └── org_structure.xlsx
│
├── process_flows/
│ ├── P2P_Flow.png
│ └── O2C_Flow.png
│
└── presentation/
└── NovaTex_SAP_Presentation.pptx
