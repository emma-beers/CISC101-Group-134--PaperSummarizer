New Feature: Summary Levels
Add this variable at start:
- summary_level = "short" or "detailed" (default: "detailed")

### Updated Logic
FOR each section:
  IF summary_level = "short":
    Generate 1-2 sentence summary
  ELSE IF summary_level = "detailed":
    Generate paragraph + 3-5 bullet points
   
  Check word count
  Append to results

**  New Requirement A:** Add “Summary Level” Modes (Module 02)  The summarizer should support two summary levels for each section:

summary_level = "short"

1–2 sentence summary per section
summary_level = "detailed"

A short paragraph plus a bullet list of 3–5 key points for each section
You must:

Add a variable (e.g., summary_level) to the module’s logic.

Add conditional behavior in the section loop:

If summary_level = "short" → generate only a compact summary.

If summary_level = "detailed" → generate summary + bullet list.


