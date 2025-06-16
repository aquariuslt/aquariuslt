# Copilot Instructions

## Purpose
This file provides instructions for GitHub Copilot and Copilot Workspace when generating Pull Requests and Issues in this repository.

---

## 📦 PR Requirements

When Copilot creates a Pull Request, it **must**:

- Follow the [`.github/PULL_REQUEST_TEMPLATE.md`](./.github/PULL_REQUEST_TEMPLATE.md) format.
- Include a **clear title** summarizing the change (use imperative tone, e.g., "Add...", "Refactor...").
- Fill in all sections of the template, including:
    - Description of the change
    - Motivation and context
    - Related Issue(s)
    - Checklist
- Keep changes **minimal and scoped** to the problem it solves.

---

## 🧾 Issue Requirements

When Copilot creates an Issue, it should:

- Clearly state the **problem or question**.
- Include relevant **code snippets or context**.
- If clarification is needed from the maintainer:
    - Add a checklist like:

      ```md
      ### Questions for the Maintainer
      - [ ] What behavior is expected when X occurs?
      - [ ] Should we support edge case Y?
      ```

- Use labels like `needs-confirmation`, `copilot-generated`, or `triage`.


---

## Commit Message Convention

All commit messages **must** follow the [Conventional Commits](https://www.conventionalcommits.org/) format:



---

## ⚠️ Limitations

Copilot **must not**:
- Modify unrelated files in a single PR.
- Auto-approve its own PRs.
- Submit dependency updates without a clear reason.

---

## ✅ Examples

Good PR title:
> Refactor `useMiner` hook to support paginated API

Bad PR title:
> Update stuff

---

## 📬 Contact

If Copilot is unsure about the approach, it should:
- Open an Issue instead of a PR
- Add a comment like:  
  _"Unsure about requirement Z. Please confirm before continuing implementation."_



