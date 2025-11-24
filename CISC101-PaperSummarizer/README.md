# CISC 101 – Research Paper Summarizer (Group Project)

This repository contains the full modular system design for the Week 10–12 Final Project in CISC 101.

---

## Repository Structure

/
├── system_prompt.md
├── README.md
└── modules/
    ├── 01_intake_setup.md
    ├── 02_section_loop.md
    ├── 03_guardrails.md
    ├── 04_rendering_refinement.md
    ├── 05_citation_extractor.md
    └── 06_contribution_highlighter.md

---

## Overview

This project implements a complete Research Paper Summarizer with:

- PS2 specifications  
- Multi-module architecture  
- Strict evidence mode  
- Short/detailed summary modes  
- Hallucination guardrails  
- Chunking logic  
- Expert + lay summaries  
- Two student-created modules  

---

## Usage

1. Load `system_prompt.md` into Copilot as the system instruction.  
2. Provide:  
   - paper text  
   - section list  
   - target audience  
   - (optional) summary_level  
   - (optional) evidence_mode  
3. Receive structured Markdown summary following the required format.

---

## Branching Requirements

Modules 02 and 03 already include:

- summary_level logic  
- strict evidence mode  
- enhanced hallucination guardrails  

---

## Authors

CISC 101 Group #
