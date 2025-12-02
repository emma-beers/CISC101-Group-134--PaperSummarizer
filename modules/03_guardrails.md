### New Feature: Strict Evidence Mode
Add: evidence_mode = "normal" or "strict"

### Updated Logic
IF evidence_mode = "strict":
  Only use claims from paper
  If missing info: "Source text doesn't provide detail"

### New Warning Messages
IF section empty: "Section skipped: no usable text"
IF section <50 words: "Section very short: summary may be incomplete"
