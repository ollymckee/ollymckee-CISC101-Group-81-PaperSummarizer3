# Module 03 — Guardrails  
(Updated version with strict evidence mode)

## Change Log
- Added evidence_mode = "strict"  
- Added standardized warnings for missing/short sections  

---

## Responsibilities
- Prevent hallucinations  
- Enforce strict evidence mode  
- Standardize section warnings  
- Enforce chunking-based constraints  

---

## Section Warning Rules

### Missing Section
“Section skipped: no usable text was provided.”

### Short Section (<50 words)
“Section very short: summary may be incomplete.”

---

## Strict Evidence Mode

If `evidence_mode = "strict"`:

- Only include claims, results, methods, and equations present in the text  
- No domain knowledge additions  
- No inferred reasoning  
- If the text lacks enough details:  
  “The source text does not provide enough detail to summarize this section in strict evidence mode.”

---

## Hallucination Mitigation
- No invented details  
- If unsure → omit  
- If not found → explicitly say:  
  “Information not found in source text.”

---

## Output
Module returns:
- Guarded summary for each section  
- All warnings for final rendering  
