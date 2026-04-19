# AI Response Quality Review Framework

## Objective
This project evaluates how well an LLM handles financial-service style user queries and improves weak responses through structured prompt refinement.

## Use case
A support-style assistant handling:
- eligibility and qualification questions
- repayment and payment issues
- comparison requests
- incomplete or ambiguous user queries
- multi-turn follow-up prompts

## Tools
- ChatGPT
- Excel
- Google Docs

## Project scope
- 45 scenarios tested
- 4 query types: ambiguous input, missing-information case, comparison question, multi-turn follow-up prompt
- 5 evaluation dimensions: relevance, completeness, clarity, context handling, logical consistency
- 2 prompt versions used for weak-case improvement

## Evaluation method
1. A scenario bank was created to simulate realistic user-query patterns.
2. Prompt Version 1 was used to test all 45 scenarios.
3. Responses were scored in Excel across five quality dimensions.
4. Weak patterns were logged in a failure tracker.
5. Prompt Version 2 was introduced for weak scenarios.
6. Weak scenarios were retested and compared before vs after.

## Key findings
- Prompt V1 handled many incomplete queries well when the answer needed clarification first.
- Weak cases clustered around broad comparison questions and vague recommendation asks.
- Prompt V2 improved these weaker scenarios by adding:
  - clearer clarification behavior
  - stronger comparison criteria
  - better next-step structure
  - more explicit use of follow-up context

## Folder structure
```text
AI-Response-Quality-Review-Framework/
├── README.md
├── data/
│   └── AI_Response_Quality_Review_Framework_Filled.xlsx
├── docs/
│   ├── prompt_versions.md
│   ├── project_findings.md
│   ├── sample_outputs.md
│   └── response_library.md
└── screenshots/
    ├── scenario_bank_preview.png
    ├── scoring_framework_preview.png
    ├── failure_log_preview.png
    └── before_after_preview.png
```

## Key artifacts
- `data/AI_Response_Quality_Review_Framework_Filled.xlsx` - scenario bank, scoring sheet, failure log, before vs after comparison, and response library
- `docs/prompt_versions.md` - Prompt V1, Prompt V2, and the reasoning behind refinement
- `docs/project_findings.md` - summary of weak patterns and improvements
- `docs/sample_outputs.md` - sample model responses used in the project
- `docs/response_library.md` - full response list for all scenarios used in the workbook

## Notes
- The response text in the docs and workbook is aligned intentionally so the project remains internally consistent.
- For GitHub presentation, the screenshots folder contains preview images derived from the project artifacts.
