# Claude Prompting Best Practices (Simple Guide)

## 1. Be Clear and Specific

Claude works best when instructions are clear and direct.

Think of Claude like a smart new employee. It does not know your habits or expectations, so you must explain exactly what you want.

Good prompts include:

* Clear instructions
* Exact output format
* Step-by-step tasks when order matters

---

## 2. Give Context

Explain why the task matters. Context helps Claude understand your goal and produce better results.

Example:
Instead of "Format this text", say "Format this text so it can be used in a professional report."

---

## 3. Use Examples

Examples are one of the most powerful prompting techniques. Provide 3–5 examples that demonstrate the format, tone, and structure you want.

Tips:

* Make examples realistic
* Include edge cases
* Separate examples clearly from instructions

---

## 4. Structure Prompts with XML Tags

XML tags help Claude understand complex prompts.

Example structure:

```xml
<context>
Background information
</context>

<instructions>
What Claude should do
</instructions>

<examples>
Example outputs
</examples>

<input>
User input
</input>
```

---

## 5. Give Claude a Role

Setting a role improves response quality.

Example:
"You are a Python coding assistant."

This helps Claude adjust its tone, knowledge, and style.

---

## 6. Handling Large Documents

When using large documents:

1. Put documents first
2. Put instructions second
3. Put the question last

Also ask Claude to quote relevant parts before analyzing.

---

## 7. Control Output Format

Tell Claude what to do rather than what not to do.

Bad: "Do not use markdown"

Better: "Write the answer using plain paragraphs."

---

## 8. Control Behavior with System Prompts

System prompts define how Claude behaves.

Examples:

Proactive behavior:
Implement changes rather than only suggesting them.

Conservative behavior:
Only perform actions when explicitly requested.

---

## 9. Tool Usage

If tools are available, clearly instruct Claude when to use them.

Example:
Instead of "Suggest changes", say "Implement the changes."

---

## 10. Parallel Tool Execution

Claude can run tools in parallel for faster results.

Example:
Reading multiple files at the same time instead of sequentially.

---

## 11. Thinking and Reasoning

Claude can reason deeply when needed.

Adaptive thinking allows Claude to decide when deeper reasoning is necessary.

Effort levels control reasoning depth:

* Low
* Medium
* High

---

## 12. Avoid Overthinking

Sometimes Claude explores too many options. You can guide it by asking it to choose one approach and commit to it.

---

## 13. Use Self-Checking

Ask Claude to verify its work before finishing.

Example:
"Before finishing, check your answer against the requirements."

---

## 14. Agent Workflows

Claude can perform long multi-step tasks like an autonomous agent.

Best practices:

* Track progress
* Work incrementally
* Save state

Example files:

* progress.txt
* tests.json

---

## 15. Safety for Autonomous Actions

Claude may perform destructive actions if not restricted. Add instructions to confirm before actions like:

* Deleting files
* Force pushing commits
* Modifying shared systems

---

## 16. Research Tasks

For complex research:

* Gather multiple sources
* Form competing hypotheses
* Track confidence levels
* Critically evaluate findings

---

## 17. Avoid Overengineering

Claude sometimes adds unnecessary complexity.

You can instruct it to:

* Only implement requested features
* Avoid unnecessary abstractions
* Keep solutions simple

---

## 18. Prevent Hallucinations

Tell Claude to read files before answering about them.

Example rule:
"Never speculate about code you have not opened."

---

## 19. Frontend Design Guidance

To avoid generic AI designs:

* Use distinctive fonts
* Create strong color themes
* Add meaningful animations
* Avoid generic layouts

---

## 20. Claude 4.6 Migration Notes

Key changes:

* Adaptive thinking replaces older reasoning systems
* Prefilled responses are removed
* Models are more proactive
* Effort parameter controls reasoning depth

---

# Quick Rules

1. Be clear and specific
2. Give context
3. Use examples
4. Structure prompts
5. Define output format
6. Assign a role
7. Ask for self-checking

---

Good prompts are clear, structured, example-driven, and explicit about the output you want.
