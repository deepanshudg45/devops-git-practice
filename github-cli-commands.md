# GitHub CLI (gh) Commands – Day 26

## Authentication

### gh auth login
Authenticate with GitHub.
Example:
gh auth login

---

### gh auth status
Check authentication status.
Example:
gh auth status

---

# Repository Management

### gh repo create
Create a new GitHub repository.
Example:
gh repo create repo-name --public --add-readme

---

### gh repo clone
Clone repository using gh.
Example:
gh repo clone owner/repo-name

---

### gh repo view
View repository details.
Example:
gh repo view

---

### gh repo list
List your repositories.
Example:
gh repo list

---

### gh repo delete
Delete a repository.
Example:
gh repo delete repo-name --confirm

---

# Issues

### gh issue create
Create an issue from terminal.
Example:
gh issue create --title "Bug" --body "Fix needed"

---

### gh issue list
List open issues.
Example:
gh issue list

---

### gh issue view
View issue details.
Example:
gh issue view 1

---

### gh issue close
Close an issue.
Example:
gh issue close 1

---

# Pull Requests

### gh pr create
Create pull request.
Example:
gh pr create --fill

---

### gh pr list
List pull requests.
Example:
gh pr list

---

### gh pr view
View PR details.
Example:
gh pr view 1

---

### gh pr merge
Merge pull request.
Example:
gh pr merge 1 --merge

---

### gh pr checkout
Checkout PR locally.
Example:
gh pr checkout 5

---

### gh pr review
Review PR.
Example:
gh pr review 5 --approve

---

# GitHub Actions

### gh run list
List workflow runs.
Example:
gh run list

---

### gh run view
View workflow run details.
Example:
gh run view <run-id>

---

# Advanced / Automation

### gh api
Make raw GitHub API calls.
Example:
gh api repos/:owner/:repo

---

### gh gist
Create and manage gists.
Example:
gh gist create file.txt

---

### gh release create
Create release.
Example:
gh release create v1.0.0

---

### gh alias
Create shortcut commands.
Example:
gh alias set prc "pr create --fill"

---

### gh search repos
Search GitHub repositories.
Example:
gh search repos devops
