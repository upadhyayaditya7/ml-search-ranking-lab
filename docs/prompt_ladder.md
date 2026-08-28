# Prompt Ladder Assignment: ML Search-Ranking Data Validation

## 1. Baseline (Version 0)
* **Prompt:** *"Check my python code for the ml search ranking lab"*
* **Output Excerpt:** *"Here is a generic Python script for checking data. You can use pandas to read your CSV file and handle missing columns with basic try-except blocks..."*
* **Four Notes:**
  * **What changed in the prompt:** Initial lazy baseline query asking for broad code review.
  * **What actually improved in the output:** It provided a generic template, but it had zero context on the actual repository structure or CSV schemas.
  * **What still failed:** It gave completely generic boilerplate code that ignored local paths, specific error codes, and the actual dataset name.
  * **What you would try next:** Add a clear, specific goal to target the exact file validation requirements.

---

## 2. Version 1 (+ Clearer Goal)
* **Prompt:** *"Write a Python script that validates `content_refresh_anonymized.csv` for missing values and exits with `sys.exit(1)` if any errors are found."*
* **Output Excerpt:** 
  ```python
  import pandas as pd
  import sys
  
  df = pd.read_csv('content_refresh_anonymized.csv')
  if df.isnull().any().any():
      sys.exit(1)