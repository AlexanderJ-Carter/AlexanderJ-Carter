# Repository Governance

## Repository Description
Personal profile hub of AlexanderJ-Carter: projects, notes, experiments, and creative automation around software, electronics, Linux, and Verilog.

## Branch Strategy
- Default branch: main
- Feature work: short-lived branches with pull requests
- Protected branch: main

## Recommended Branch Protection for main
- Require a pull request before merging
- Require at least 1 approval
- Dismiss stale approvals when new commits are pushed
- Require conversation resolution before merging
- Require status checks to pass before merging
- Require branches to be up to date before merging
- Restrict force pushes and branch deletion
- Include administrators

## Required Status Checks
- Profile CI / markdown-lint
- Profile CI / workflow-lint

## Optional but Recommended Checks
- Link Check / lychee
- Snake build workflow health

## Branch Protection JSON Import
- JSON payload file: .github/branch-protection-main.json
- Apply with GitHub CLI:

```bash
gh api --method PUT repos/AlexanderJ-Carter/AlexanderJ-Carter/branches/main/protection --input .github/branch-protection-main.json
```

## Automation Summary
- Snake animation generation: .github/workflows/snake.yml
- Profile quality checks: .github/workflows/profile-ci.yml
- Link validation: .github/workflows/link-check.yml
- Release draft generation: .github/workflows/release-drafter.yml
- PR auto labeling: .github/workflows/pr-labeler.yml
- Dependency updates: .github/dependabot.yml

## Contribution Entry Points
- Bug report form: .github/ISSUE_TEMPLATE/bug-report.yml
- Idea proposal form: .github/ISSUE_TEMPLATE/idea-proposal.yml
- Pull request template: .github/pull_request_template.md
