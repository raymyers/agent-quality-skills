---
name: review
description: Test quality scoring using Dave Farley's 8 properties (Farley Score). Use when reviewing a test suite for quality, maintainability, and TDD adherence.
---
# Review

## Dave Farley's 8 Properties

Score each 1–10, calculate:

**Farley Score** = `(U×1.5 + M×1.5 + R×1.25 + A + N + G + F×0.75 + T) / 9`

| # | Property | Weight | Key question |
|---|---|---|---|
| U | Understandable | 1.5× | Does this read like a specification? |
| M | Maintainable | 1.5× | Do implementation changes break these tests? |
| R | Repeatable | 1.25× | Same result every time, anywhere? |
| A | Atomic | 1× | Completely isolated; no shared state; parallelizable? |
| N | Necessary | 1× | Does every test add unique value? |
| G | Granular | 1× | Does each test assert exactly one thing? |
| F | Fast | 0.75× | Milliseconds, not seconds? |
| T | First (TDD) | 1× | Evidence of test-first approach? |

**Score bands**: <4.5 critical · 4.5–6.0 fair · 6.0–7.5 good · 7.5–9.0 excellent · 9.0+ exemplary

**Output format**:
```
## Test Design Review: [File/Suite Name]

| Property | Score | Evidence |
|---|---|---|
| Understandable | X/10 | ... |
...

### Farley Score: X.X/10 [Band]

### Top Recommendations
1. [Highest-impact improvement]
2. ...
```

Reference: https://www.linkedin.com/pulse/tdd-properties-good-tests-dave-farley-iexge/

---

## Checklist

- [ ] Each property scored with specific evidence from the code
- [ ] Farley Score calculated and band identified
- [ ] Top recommendations prioritised by impact
