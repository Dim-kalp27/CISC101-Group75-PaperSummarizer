# Change Log (2025-03-10)
- Added strict evidence mode
- Added standardized warning messages
- Strengthened hallucination mitigation

# Module 03 — Guardrails

evidence_mode options:
- "strict"
- "normal"

If evidence_mode = "strict":
- Only include claims, equations, and results found directly in the provided text.
- If insufficient detail exists:
  Output: “The source text does not provide enough information to summarize this section in strict evidence mode.”

Warning Rules:
If a section is missing:
  Output: “Section skipped: no usable text was provided.”

If section contains <50 words:
  Output: “Section very short: summary may be incomplete.”

Hallucination Mitigation:
- Do not invent citations.
- Do not invent math or results.
- Do not create content not supported by the paper.
- No expansions beyond provided text.
