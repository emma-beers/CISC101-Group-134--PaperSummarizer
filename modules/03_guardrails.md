### New Feature: Strict Evidence Mode
Add: evidence_mode = "normal" or "strict"

### Updated Logic
IF evidence_mode = "strict":
  Only use claims from paper
  If missing info: "Source text doesn't provide detail"

### New Warning Messages
IF section empty: "Section skipped: no usable text"
IF section <50 words: "Section very short: summary may be incomplete"


**New Requirement B**: Strengthen Evidence & Hallucination Guardrails (Module 03)

Strict Evidence Mode: Introduce a mode or flag (e.g., evidence_mode = "strict"). When it is set to "strict":

The summarizer should:

Only include claims, equations, and results that appear in the provided text.

If it cannot find enough information, it must say so explicitly (e.g., “The source text does not provide enough detail to summarize this section in strict evidence mode.”).

Section Warning Messages For sections that are:

missing / empty, or

too short (< 50 words)

The module must instruct the system to output a standardized warning, such as:

“Section skipped: no usable text was provided.”

“Section very short: summary may be incomplete.” You decide the exact wording.
