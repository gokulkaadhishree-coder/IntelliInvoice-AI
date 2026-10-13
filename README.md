# IntelliInvoice AI 🧾🤖
### Agentic AI-Powered Invoice Processing and Discrepancy Detection

## 📌 Overview

**IntelliInvoice AI** is an intelligent invoice processing solution built using UiPath Agentic AI and workflow orchestration. It automates invoice data extraction, validates invoice details against purchase orders, investigates discrepancies, and routes cases for human review when required.

By combining AI agents, business process automation, and human-in-the-loop approval, the system aims to make invoice verification more efficient, consistent, and reliable.

## 🎯 Problem Statement

Manual invoice processing can be time-consuming and prone to errors. Businesses must verify invoice amounts, vendor details, quantities, taxes, and contractual terms before approving payments. Mismatches can lead to incorrect payments, delayed processing, and additional administrative work.

IntelliInvoice AI addresses this challenge by automating invoice verification and assisting with discrepancy investigation.

## ✨ Key Features

- **Automated Invoice Intake:** Monitors incoming invoice emails through Gmail integration.
- **AI-Powered Data Extraction:** Extracts relevant invoice information, including invoice number, vendor details, dates, line items, and totals.
- **Purchase Order Matching:** Compares extracted invoice information with available purchase order records.
- **Discrepancy Detection:** Identifies potential mismatches in quantities, prices, totals, and vendor information.
- **AI-Assisted Investigation:** Uses available vendor contract information and contextual grounding to investigate discrepancies.
- **Human-in-the-Loop Approval:** Routes cases for human review before important decisions are finalized.
- **Automated Email Generation:** Generates professional email responses based on investigation findings.
- **Workflow Orchestration:** Coordinates agents, automation workflows, and review tasks using UiPath Maestro.

## 🔄 Workflow

1. **Invoice Reception:** An invoice arrives through the connected Gmail account.
2. **Data Extraction:** An AI agent extracts relevant invoice fields.
3. **Purchase Order Retrieval:** The workflow retrieves the corresponding purchase order information.
4. **Invoice Validation:** Invoice details are compared against purchase order records.
5. **Discrepancy Investigation:** The system investigates identified mismatches using available contextual information.
6. **Human Review:** Cases requiring approval are presented to a reviewer.
7. **Email Generation:** An AI agent prepares an appropriate response based on the case outcome.
8. **Communication:** The workflow sends or prepares the email through the configured Gmail integration.

## 🛠️ Technology Stack

- **UiPath Studio Web** — Workflow development
- **UiPath Agentic AI** — Intelligent data analysis and investigation
- **UiPath Maestro** — Business process orchestration
- **UiPath Data Service** — Purchase order data management, where configured
- **Gmail Integration** — Invoice intake and email communication
- **Context Grounding / RAG** — Access to relevant vendor contract information, where configured
- **Human-in-the-Loop** — Review and approval of flagged cases

## 🏗️ Core Components

| Component | Responsibility |
|---|---|
| Invoice Intake Workflow | Handles incoming invoice emails |
| Invoice Extraction Agent | Extracts structured information from invoices |
| Purchase Order Matching | Compares invoice data against purchase order records |
| Discrepancy Investigation Agent | Investigates mismatches and supporting evidence |
| Human Review Workflow | Enables review of cases requiring intervention |
| Email Generation Agent | Drafts email responses |
| UiPath Maestro | Coordinates the overall process |

## 💡 Example Use Case

Suppose a vendor submits an invoice for ₹50,000, but the corresponding purchase order records ₹45,000.

IntelliInvoice AI can:

- Extract the invoice amount and purchase order details.
- Detect the ₹5,000 difference.
- Investigate the mismatch using available supporting records.
- Route the case to a human reviewer.
- Prepare an email requesting clarification or communicating the review outcome.

The system assists with verification rather than automatically treating every discrepancy as fraud.

## 🚀 Benefits

- Reduces repetitive manual invoice verification.
- Helps identify billing discrepancies earlier.
- Improves consistency in invoice processing.
- Supports faster investigation and communication.
- Maintains human oversight for important financial decisions.
- Demonstrates the integration of Agentic AI with business process automation.

## 🔮 Future Enhancements

- Add invoice status dashboards and analytics.
- Support additional invoice formats and languages.
- Introduce duplicate invoice detection.
- Add audit trails and role-based access control.
- Integrate ERP and accounting systems.
- Improve exception handling and validation rules.
- Add automated reporting for invoice discrepancies.

## ⚙️ Setup and Configuration

This project is developed using UiPath Studio Web and its configured integrations.

To reproduce the workflow:

1. Access a compatible UiPath Automation Cloud environment.
2. Import or open the project in the appropriate UiPath workspace.
3. Configure the required Gmail, data, and AI connections.
4. Set up the required purchase order records and vendor contract reference data.
5. Configure agent instructions, permissions, and human-review tasks.
6. Test the workflow using sample invoices before processing real financial documents.

Exact setup requirements depend on the project configuration and enabled UiPath services.

## 🔐 Security Considerations

- Store credentials securely using approved credential-management facilities.
- Avoid committing API keys, passwords, tokens, or sensitive invoice data to GitHub.
- Restrict access to financial documents and vendor records.
- Validate AI-generated findings before making payment decisions.
- Use human approval and audit logging for sensitive actions.

## ⚠️ Disclaimer

IntelliInvoice AI is intended for educational and demonstration purposes. AI-generated findings may be inaccurate and should be validated against authoritative financial records. The solution should not independently authorize payments without appropriate business controls.

## 📂 Project Information

**Project Name:** IntelliInvoice AI  
**Domain:** Financial Process Automation  
**Focus Areas:** Agentic AI, Invoice Processing, Discrepancy Detection, Human-in-the-Loop Automation  
**Platform:** UiPath Automation Cloud

---

*Built to explore how Agentic AI and workflow orchestration can simplify invoice verification and financial operations.*
