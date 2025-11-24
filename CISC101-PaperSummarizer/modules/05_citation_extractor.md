# Module 05 — Citation Extractor

## Responsibilities
- Identify citation markers within text  
- Extract only citations explicitly present  
- Provide them to the rendering layer  

---

## Workflow
1. Detect in-text patterns such as:  
   - [1], [2], [14]  
   - (Author, 2020)  
   - Author et al. (2017)  
2. Extract citations in order of appearance  
3. Return them as a list  
4. If none found → return empty list  

---

## Guardrails
- Do not invent citations  
- Do not fabricate bibliographic entries  
