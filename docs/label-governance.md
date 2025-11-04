# Label Governance

This document describes how we manage and evolve the repository's labels.

---

## What Each Label Means

We use three primary labels to indicate the impact and type of changes:

- **major** (`#f44336`)
  - **Description:** Backward-incompatible or breaking changes.
  - Introduces changes that require users or contributors to update their workflows, integrations, or code.
- **minor** (`#4caf50`)
  - **Description:** Backward-compatible feature additions.
  - Adds new functionality or improvements that do not break existing usage.
- **patch** (`#2196f3`)
  - **Description:** Backward-compatible bug fixes or trivial changes.
  - Fixes bugs or makes small updates that do not affect functionality or public APIs.

---

## How to Propose Changes

If you want to propose edits, removals, or additions to our label set:

1. **Open a Pull Request**
   - Edit the [`labels.yml`](../labels.yml) file with your proposed changes.
   - Optionally, update this document to explain any new or modified labels.
2. **Describe Your Rationale**
   - Include a clear explanation of why the change is needed.
   - If proposing a new label, provide its purpose, color, and description.
3. **Review Process**
   - Proposals will be discussed in the PR.
   - The DevEx team (`@legalclaimassistant/devex`) is responsible for final review and approval.

Label changes are enforced and synced automatically via our [label sync workflow](../workflows/label-sync.yml).

---

## Color + Description Standard

When adding or changing a label:

- **Color:** Choose a color that is visually distinct from existing labels and reflects the label's purpose (e.g., red for breaking changes, green for enhancements, blue for patches/bug fixes).
- **Description:** Keep descriptions short, clear, and actionable. They should help all contributors quickly understand the purpose of each label.

**Example:**
```yaml
- name: major
  color: f44336
  description: Backward-incompatible or breaking changes
```

Please refer to `labels.yml` for the complete and canonical list of labels and their properties.

