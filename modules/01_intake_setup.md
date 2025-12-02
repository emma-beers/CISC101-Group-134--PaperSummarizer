Module 1: Intake & Setup

**Purpose**
Normalize paper sections and detect missing/short content.

**Inputs**
- Raw paper text
- Section list (provided by user)

## Process
1. Split text into sections based on headers
2. Check for missing sections
3. Flag sections with < 50 words
4. Normalize formatting

## Output
- Normalized section array
- Warnings for problematic sections
