# POS Checkout Tax Exemption Feature

BRD, use case, and wireframes for a POS checkout feature that removes tax for non-profit customers.

## Business Problem
At checkout, cashiers cannot remove tax for customers with a non-profit business account. The business is losing sales from these customers.

## Proposed Solution
Let the cashier enter the customer's tax-exempt ID at checkout. If the ID is valid, the system removes the tax from the purchase.

## Business Requirements
- **BR1:** The cashier can enter a non-profit tax ID.
- **BR2:** The manager can approve or cancel a tax-exemption request.

**Business rule:** Manager approval is required only when the tax-exempt amount is greater than $50.

## What's Included
- **BRD:** business problem, proposed solution, requirements, and business rules
- **Use Case Document:** actors, main flow, alternate flows, and exceptions
- **Wireframes:** 7 screens covering the success and error scenarios

| File | Contents |
|---|---|
| `BRD.docx` | Business Requirements Document |
| `Use_Case_Tax_Exempt.docx` | Use case with flows and field specifications |
| `Wireframe_1` to `Wireframe_7` | Screens for the main flow and error scenarios |

## Use Case Summary
**Use Case:** Enter Tax-Exempt ID
**Actors:** Cashier, Manager

| Flow | Scenario |
|---|---|
| Primary flow | Cashier enters a valid tax-exempt ID and the system removes the tax |
| Alternate flow 1 | Invalid Tax-ID format |
| Alternate flow 2 | Tax amount above $50, so manager approval is required |
| Alternate flow 3 | Invalid manager User ID or PIN |
| Exception flow 1 | Cashier or manager cancels |
| Exception flow 2 | Entered ID is not tax-exempt |

## Field Validation Rules
- **Tax-Exempt ID:** numeric, 10 characters, required
- **Manager User ID:** alphanumeric, 5 characters, required
- **Manager PIN:** numeric, 4 digits, required, encrypted

## Tools Used
[Your wireframing tool], Microsoft Word

## Note
This is a practice project built on a sample Vend POS screen. It is not client work.
