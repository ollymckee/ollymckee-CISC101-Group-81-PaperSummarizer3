# Module 02 — Section Loop  
(Updated version with summary-level logic)

## Change Log
- Added summary_level variable (“short” / “detailed”)  
- Implemented conditional summary behavior for each mode  

---

## Responsibilities
- Iterate through each section in normalized list  
- Extract section text  
- Summarize according to summary_level  
- Add warnings where needed  
- Forward to guardrails before final rendering  

---

## Summary-Level Logic

### summary_level = "short"
- Produce a 1–2 sentence summary  
- No bullet list  

### summary_level = "detailed"
- Produce a short paragraph  
- Followed by 3–5 bullet points  
- Key ideas must be extracted directly from text  

---

## Loop Algorithm

For each section **S**:

1. Extract `S_text`  
2. If section missing:  
   - Output: “Section skipped: no usable text provided.”  
   - Move to next section  
3. If section <50 words:  
   - Add warning: “Section very short: summary may be incomplete.”  
4. Summarize based on summary_level rules  
5. Pass result + warnings to Module 03  
6. Store completed section for rendering  
