# Change Log (2025-03-10)
- Added summary_level variable
- Added short mode (1–2 sentence summaries)
- Added detailed mode (paragraph + 3–5 bullet points)

# Module 02 — Section Loop

summary_level options:
- "short"
- "detailed"

For each section:
1. Confirm the section contains text.
2. If section text <50 words → send to Guardrails.
3. Summarize using only the provided text.

If summary_level = "short":
- Produce a compact 1–2 sentence summary.

If summary_level = "detailed":
- Produce a paragraph (100–150 words).
- Include a bullet list of 3–5 key points extracted ONLY from the text.

All summaries must maintain:
- Chronological order  
- Academic tone  
- Consistent terminology  
- No invented citations, equations, or claims

