# Module 01 — Intake & Setup

## Responsibilities
- Validate and store user inputs  
- Normalize section names  
- Identify missing / empty / <50-word sections  
- Detect long-paper conditions and apply chunking strategy  
- Initialize summary_level and evidence_mode variables  
- Prepare internal data structures for Section Loop

---

## Workflow

1. Receive and validate all inputs  
2. Normalize section names (case-insensitive, strip punctuation)  
3. Match user-provided section list to actual paper text  
4. Mark any missing sections  
5. Check for empty or <50-word sections  
6. If paper is larger than context window → apply chunking plan  
7. Pass cleaned data to Module 02  
