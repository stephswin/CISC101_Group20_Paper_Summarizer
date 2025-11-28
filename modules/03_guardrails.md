# Module 3: Guardrails

Missing/Empty Sections: Insert placeholder + warning.  
Short Sections (<50 words): Flag for user review.  
Hallucination Mitigation: Summarize only from provided text.  
Long-Paper Chunking: Break into manageable chunks using PS2 context-window strategies.

---

## New Requirement B: Strengthened Evidence & Hallucination Guardrails

### Strict Evidence Mode
Add variable: **`evidence_mode` ∈ {"strict", "default"}`**

- **If `evidence_mode = "strict"`**
  - Only include claims, equations, and results that explicitly appear in the provided text.
  - If insufficient information is available, the system must output a standardized message such as:  
    **“Insufficient information: the source text does not provide enough detail to summarize this section in strict evidence mode.”**

### Section Warning Messages
For sections that are **missing**, **empty**, or **<50 words**, output standardized warnings, for example:

- **“Section skipped: no usable text was provided.”**  
- **“Section very short: summary may be incomplete.”**

These warnings must appear in the section’s corresponding output fields.
