 1. Core Workflow & Daily Habits

Work in Feature Branches:** Avoid committing directly to the main branch (main or master). Create descriptive feature branches for new work:
bash
git checkout -b feature/user-authentication

Make Small, Atomic Commits: Commit small, logical chunks of code rather than one massive commit at the end of the day. Write clear, imperative commit messages (e.g., Add user login validation, not updated stuff).
Pull Before You Push: Keep your local branch up-to-date with remote changes to avoid merge conflicts:
bash
git pull origin main


2. Collaboration & Code Quality

Use Pull Requests (PRs): Submit PRs to propose changes. PRs provide a dedicated space to discuss changes, view diffs, and run automated tests.
Conduct Code Reviews:Require at least one peer review before merging code into main to maintain code standards and share project knowledge across the team.
Protect Core Branches: Go to Settings > Branches in your repository and set up Branch Protection Rules to prevent direct pushes to main and require passing status checks and reviews before merging.


 3. Project Management & Organization

Leverage Issues & Labels:Track bugs, feature requests, and tasks using GitHub Issues. Apply labels (e.g., bug, enhancement, documentation) and assign them to specific team members.
Link Commits and PRs to Issues: Mention issue numbers in your commit messages or PR descriptions (e.g., Fixes #12 or Closes #45) to automatically close issues when the code is merged.
Use GitHub Projects: Organize tasks using Kanban boards or roadmaps inside the Projects tab to visualize sprint progress.

 4. Documentation & Repository Health

Maintain a Comprehensive README.md: Include project overview, installation steps, prerequisite requirements, and usage examples so new contributors can get started quickly.
Add a .gitignore File: Exclude build files, environment variables, secret keys (.env), and node modules/dependencies from tracked files.
Provide `CONTRIBUTING.md & Issue Templates: If working on open-source or large team projects, create issue and pull request templates to ensure contributors provide essential context.



5. Security & Automation

Never Commit Secrets: Use GitHub Secrets (`Settings > Secrets and variables) for API keys, passwords, and tokens.
Automate with GitHub Actions: Set up CI/CD pipelines to automatically build, test, and deploy code whenever a pull request is opened or merged.
Enable Dependabot: Keep security vulnerabilities at bay by allowing Dependabot to scan dependencies and automatically create pull requests for outdated packages.
