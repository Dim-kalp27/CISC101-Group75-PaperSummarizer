# Research Paper Summarizer

This project implements a structured summarizer for research papers, designed around the PS2 specification.

## Features
- Summarizes each section in **100–150 words**.
- Produces a **final summary ≤400 words**.
- Generates both **expert** and **layperson** summaries.
- Includes a **mini-glossary** of technical terms.
- Provides **checks & warnings** for missing or short sections.
- Extracts **key contributions** (3–5 points).
- Explains **equations and technical terms** in simple language.

## Module Architecture
1. **Intake & Setup** — Normalize sections, detect issues, chunk text.
2. **Section Loop** — Summarize each section with PS2 constraints.
3. **Guardrails** — Prevent hallucinations, enforce evidence rules.
4. **Rendering & Refinement** — Format outputs and ensure clarity.
5. **Key Contributions Extractor** — Highlight main contributions.
6. **Equation & Technical Term Explainer** — Simplify technical content.

## Usage
Provide:
1. Full text of the paper (*e.g., Attention Is All You Need*).
2. Section titles and boundaries.
3. Target audience (expert or lay).

The system will return:
- Paper Summary
- Section-by-Section Summary Table
- Expert Summary
- Lay Summary
- Mini-Glossary
- Checks & Warnings
