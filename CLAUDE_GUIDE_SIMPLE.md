# Writing a Good CLAUDE.md (Simple Explanation)

## 1. AI Models Don't Remember Your Code

AI coding tools like Claude **do not remember anything between sessions**.

Every time you start a new chat:
- The AI knows **nothing about your codebase**
- It only knows the **information you provide**

Because of this, developers use a file called **`CLAUDE.md`**.

This file acts like a **quick guide that explains your project to the AI**.

---

# 2. What a Good CLAUDE.md Should Contain

Your file should explain **three important things**.

## WHAT
Explain the **technology and structure of the project**.

Example:
- Frameworks used
- Folder structure
- Applications in the repository

Example:
- Frontend: React
- Backend: Django
- Database: PostgreSQL


This helps the AI understand **where things are located**.

---

## WHY
Explain the **purpose of the project**.

Example:
- What the system does
- Why different parts exist

Example:
- The backend handles API requests.
- The frontend displays the user interface.

This helps the AI understand **the role of each component**.

## HOW
Explain **how the AI should work with the project**.

Examples:
- How to run the project
- How to run tests
- How to check if code works

Example:
- Run tests with: npm test
- Build project with: npm run build


This allows the AI to **verify its own changes**.

---

# 3. Keep the File Short

Many people make the mistake of adding **too many instructions**.

AI models can only follow **around 150–200 instructions effectively**.

If there are too many instructions:
- The AI may ignore them
- Performance becomes worse

Best practice:
- Keep `CLAUDE.md` **small and focused**

Recommended size:
- Under 300 lines



Some teams use **less than 60 lines**.

---

# 4. Claude May Ignore Your File

Claude is designed to **ignore instructions that are not relevant**.

Example:

If the AI is fixing a UI bug, it may ignore instructions about:
- database schema
- backend architecture

Therefore:

Your `CLAUDE.md` should contain **only information useful for most tasks**.

---

# 5. Use Progressive Disclosure

Instead of putting everything inside `CLAUDE.md`, create **separate documentation files**.

Example structure:
agent_docs/
  - building_project.md
  - running_tests.md
  - code_conventions.md
  - architecture.md

    
Then in `CLAUDE.md` you simply reference them.

Example:
- If you need to run tests, read agent_docs/running_tests.md
- If you need architecture information, read agent_docs/architecture.md

This keeps the main file **clean and easy to understand**.

---

# 6. Don't Use AI for Code Formatting

Some developers put **code style rules** inside `CLAUDE.md`.

This is not recommended.

Instead, use tools such as:

- ESLint
- Prettier
- Biome

These tools are:
- Faster
- More reliable
- Better for formatting code

AI should focus on **logic and implementation**, not formatting.

---

# 7. Don't Auto-Generate CLAUDE.md

Some tools can automatically create a `CLAUDE.md` file.

However, this can lead to **bad instructions**.

Since this file affects **every AI session**, it is better to:

- Write it manually
- Carefully review every line

---

# Key Takeaways

A good `CLAUDE.md` file should:

1. Explain **WHY, WHAT, and HOW** of your project  
2. Stay **short and focused**  
3. Contain only **important instructions**  
4. Move detailed info to **separate docs**  
5. Use **linters instead of AI for formatting**  
6. Be **written carefully by developers**

---

# Simple Summary

`CLAUDE.md` is a **small guide that explains your project to an AI coding assistant so it can work correctly with your codebase.`


This keeps the main file **clean and easy to understand**.

---

# 6. Don't Use AI for Code Formatting

Some developers put **code style rules** inside `CLAUDE.md`.

This is not recommended.

Instead, use tools such as:

- ESLint
- Prettier
- Biome

These tools are:
- Faster
- More reliable
- Better for formatting code

AI should focus on **logic and implementation**, not formatting.

---

# 7. Don't Auto-Generate CLAUDE.md

Some tools can automatically create a `CLAUDE.md` file.

However, this can lead to **bad instructions**.

Since this file affects **every AI session**, it is better to:

- Write it manually
- Carefully review every line

---

# Key Takeaways

A good `CLAUDE.md` file should:

1. Explain **WHY, WHAT, and HOW** of your project  
2. Stay **short and focused**  
3. Contain only **important instructions**  
4. Move detailed info to **separate docs**  
5. Use **linters instead of AI for formatting**  
6. Be **written carefully by developers**
