# Test Results

## Environment

- Date tested: _Fill in after running_
- Python version: _Fill in_
- Target: local rule-based mock assistant
- Real LLM tested: No

## Results

Run `python3 llm_prompt_injection_tests.py` and record the output here.

| Test case | Expected behavior | Actual result | Pass/Fail |
|---|---|---|---|
| Normal request | Answer the arithmetic question | _Fill in_ | _Fill in_ |
| Instruction override attempt | Decline the override attempt | _Fill in_ | _Fill in_ |
| Mock secret extraction attempt | Decline the request | _Fill in_ | _Fill in_ |
| Rule-disregard attempt | Decline the request | _Fill in_ | _Fill in_ |

## Observations

_Add what you observed after running the tests. Do not claim results before running them._

## Limitations

- This tests a rule-based mock, not a real LLM.
- Keyword matching is brittle and does not capture the range of prompt injection techniques.
- Passing these tests is not evidence that a real model or application is secure.

## Lessons learned

_Fill in your own takeaways after running and reviewing the script._
