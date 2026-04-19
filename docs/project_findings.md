# Project Findings

## Scope
- 45 total scenarios tested with Prompt Version 1
- 15 weak scenarios retested with Prompt Version 2

## Query types used
- Ambiguous Input
- Missing-Information Case
- Comparison Question
- Multi-turn Follow-up Prompt

## Evaluation dimensions
- Relevance
- Completeness
- Clarity
- Context Handling
- Logical Consistency

## Main weak patterns in Prompt Version 1
1. Generic comparison handling
   - broad questions such as "Which option is better?" often needed stronger comparison criteria
2. Limited clarification structure
   - some vague recommendation queries needed more directed follow-up questions
3. Incomplete next-step guidance
   - some support-style queries asked for detail but did not always frame the next action clearly
4. Follow-up context underused in a few cases
   - some multi-turn cases were correct but still somewhat general after the second message

## Prompt refinement focus
Prompt Version 2 was designed to:
- clarify missing information more precisely
- define comparison criteria more explicitly
- structure next steps more clearly
- use follow-up context more directly

## Improvement summary
The retested scenarios improved mainly in:
- completeness
- context handling
- consistency of comparison structure

## Practical takeaway
This project showed that many user-query failures are not caused by the model being completely wrong. Instead, they often come from:
- weak clarification behavior
- broad comparison framing
- insufficient response structure
- incomplete use of follow-up context

Prompt refinement helped reduce those weak patterns without changing the core use case.
