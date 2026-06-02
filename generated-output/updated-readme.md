## Automated Documentation Pipeline

### Overview

This feature introduces an automated documentation generation system that monitors the repository for pull request merges. When a PR is merged into the main branch, the system automatically generates updated documentation and commits it to the repository.

### What It Does

- Listens for pull request merge events via GitHub Webhooks.
- Fetches the full code diff for the merged PR using the GitHub API.
- Analyzes the changes using an LLM to understand the feature's purpose and impact.
- Generates a structured documentation section and appends it to this README.
- Commits the updated README back to the repository.

### How to Use

No manual action is required. The documentation pipeline runs automatically whenever a pull request is merged. To verify that it is working:

1. Create a feature branch with your changes.
2. Open a pull request to the main branch.
3. Merge the pull request.
4. Check the README — a new section documenting your feature will appear within seconds.

### Configuration

The pipeline is configured through the n8n workflow. To modify the documentation format or add new output types, edit the corresponding nodes in the workflow editor.

---

*This section was automatically generated and appended by the Documentation Lifecycle Agent.*
