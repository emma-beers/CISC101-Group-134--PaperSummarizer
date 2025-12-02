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
