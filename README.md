# Group Home Survey Document Generator (AI Agent)

## Overview
This repository contains an AI agent designed to **generate survey-ready compliance documents for group homes** based on a defined document requirement and known information about the home.

The agent does **not** perform full audits or continuous monitoring.  
Its sole responsibility is:

> **Given a document requirement, generate a compliant, customized document for the specific group home.**

This tool is intended to support preparation for **government surveys and licensing reviews** (e.g., MN 144G / 245D–style programs or similar regulatory frameworks).

---

## What This Agent Does

### Input
- A **document requirement** (e.g., “Emergency Preparedness Plan”)
- A structured **Home Profile** containing verified information about the group home
- Optional reference policies or templates

### Output
- A **custom, survey-ready document** populated with:
  - The home’s real operational details
  - Program-specific language
  - Proper structure and headings
- A clearly marked section listing:
  - Sources used
  - Assumptions made
  - Fields requiring human review or confirmation

---

## Example Use Cases
- “Generate our Missing Resident Protocol for this home.”
- “Create an Emergency Preparedness Plan customized to our address, staffing, and contacts.”
- “Produce a Staff Training Matrix using our staffing model.”
- “Create a Corrective Action Plan document for a survey finding.”

---

## Repository Structure

```text
/
├── home_profile/
│   └── HomeProfile.json
│
├── requirements/
│   └── document_requirements.json
│
├── templates/
│   ├── emergency_preparedness.md
│   ├── missing_resident_protocol.md
│   ├── training_matrix.md
│   └── corrective_action_plan.md
│
├── generated/
│   └── documents/
│
├── agent/
│   ├── system_prompt.md
│   ├── document_generator.py
│   └── validators.py
│
└── README.md

