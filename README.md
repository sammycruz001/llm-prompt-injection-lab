# LLM Prompt Injection Testing Lab

## Overview

This is a beginner educational project for learning how to structure tests for
prompt-injection-style inputs. It uses a **local, rule-based mock assistant** so
the tests can run without an API key, network access, or a third-party model.

## What this project demonstrates

- Organizing test cases with prompts and expected outcomes
- Checking responses against simple assertions
- Recording pass/fail results
- Recognizing the limitations of toy tests

## What it does not demonstrate

The mock assistant is not a real large language model. Its keyword rules are
deliberately simple and can be bypassed by many variations of wording. Results
from this project must not be presented as proof that a production AI system is
secure, or as testing performed against a real model.

## Requirements

- Python 3.9 or newer
- No third-party packages required

## Run the tests

From this repository directory, run:

```bash
python3 llm_prompt_injection_tests.py
```

Review the printed test results. If you change the test cases or mock assistant,
run the script again and update `results.md` with the results you actually observe.

## Methodology

Each test case contains:
1. A descriptive name
2. An input prompt
3. An expected response substring
4. A check that the demo-only mock secret is not present in the response

The current checks are illustrative, not a comprehensive security evaluation.

## Ethical scope

This starter project runs locally and uses a fake secret for demonstration.
Only test systems you own or have explicit permission to assess.

## Next steps

A future version could test a model that you are authorized to use, add a
structured test report, and evaluate additional categories such as instruction
hierarchy, untrusted input handling, and refusal consistency. Document the model,
version, configuration, test date, and limitations whenever real model testing
is performed.
