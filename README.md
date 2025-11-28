The Research Paper Summarizer is a modular system designed to process academic papers and produce structured summaries. It generates outputs for both expert and lay audiences, ensuring clarity, accuracy, and adherence to constraints defined in the specifications.

Features:
Paper Summary: Concise overall overview of the paper.
Section-by-Section Table: Structured summaries with citations and warnings.
Expert + Lay Summaries: Dual-level explanations for researchers and general readers.
Mini-Glossary: Definitions of key terms and concepts.
Checks & Warnings: Flags missing, short, or empty sections.

Modules:
Module 1: Intake & Setup – Normalizes sections, detects missing/short sections.
Module 2: Section Loop – Summarizes each section while respecting length/order constraints.
Module 3: Guardrails – Prevents hallucinations, flags short sections, handles long-paper chunking.
Module 4: Rendering & Refinement – Assembles final output with consistent formatting.
Module 5: Citation Extractor – Identifies and attaches bibliographic details.
Module 6: Equation Explainer – Detects and explains mathematical expressions in plain language.
