# Copilot Instructions

## Purpose
This file provides instructions for GitHub Copilot and Copilot Workspace when generating Pull Requests and Issues in this repository.

---

## 📦 PR Requirements

When Copilot creates a Pull Request, it **must**:

- Follow the [`.github/PULL_REQUEST_TEMPLATE.md`](./.github/PULL_REQUEST_TEMPLATE.md) format.
- Include a **clear title** following [Conventional Commits](https://www.conventionalcommits.org/) format (e.g., "feat(auth): add OAuth2 support", "fix(api): handle null responses").
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

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Types
- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation only changes
- **style**: Changes that do not affect the meaning of the code
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **test**: Adding missing tests or correcting existing tests
- **chore**: Changes to the build process or auxiliary tools

### Examples

**Good commit messages:**
```
feat(auth): add OAuth2 authentication
fix(api): handle null response in user endpoint
docs(readme): update installation instructions
chore(deps): update dependencies to latest versions
```

**Bad commit messages:**
```
Update stuff
Fix bug
Add feature
```



---

## ⚠️ Limitations

Copilot **must not**:
- Modify unrelated files in a single PR.
- Auto-approve its own PRs.
- Submit dependency updates without a clear reason.

---

## ✅ Examples

**Good PR titles:**
> feat(mining): add pagination support to `useMiner` hook
> fix(auth): resolve OAuth2 token refresh issue
> docs(api): update endpoint documentation

**Bad PR titles:**
> Update stuff
> Fix bug
> Refactor code

---

## 📬 Contact

If Copilot is unsure about the approach, it should:
- Open an Issue instead of a PR
- Add a comment like:  
  _"Unsure about requirement Z. Please confirm before continuing implementation."_



