---
name: Remediation Task
about: Track the fix for a previously identified vulnerability
title: "[FIX] <short description of fix>"
labels: remediation, fix
assignees: ""
---

## Remediation Details

**Fixes Issue:** #<!-- link to the vulnerability report issue -->  
**Finding ID:** VULN-XXX  
**Developer:** @<!-- assign to yourself -->  

---

## Root Cause

<!-- What was the underlying cause of the vulnerability? -->

---

## Fix Implemented

<!-- Describe exactly what was changed to address the vulnerability -->

**Files modified:**
- `app/app.py` — 
- `app/templates/` — 

**Before (vulnerable code):**

```python
# Paste the vulnerable code snippet here
```

**After (fixed code):**

```python
# Paste the fixed code snippet here
```

---

## Verification

**Re-test method:** <!-- How did you verify the fix works and the vulnerability is gone? -->

**Before fix — tool output:**
```
# Paste relevant Bandit / Semgrep / ZAP finding here
```

**After fix — tool output:**
```
# Paste the clean output after remediation
```

**Manual re-test evidence:** <!-- screenshot or description showing the exploit no longer works -->

---

## Regression Check

- [ ] Existing functionality still works after the fix
- [ ] SAST workflow passes with no new findings
- [ ] SCA workflow passes
- [ ] App runs successfully in Docker

---

> Remember to link this commit to the issue:
> `git commit -m "Fixes #<vulnerability_issue_number>: <description>"`
