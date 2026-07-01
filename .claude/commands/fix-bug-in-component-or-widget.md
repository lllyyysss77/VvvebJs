---
name: fix-bug-in-component-or-widget
description: Workflow command scaffold for fix-bug-in-component-or-widget in VvvebJs.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /fix-bug-in-component-or-widget

Use this workflow when working on **fix-bug-in-component-or-widget** in `VvvebJs`.

## Goal

Fixes bugs related to video embedding or similar features in builder components or widgets.

## Common Files

- `libs/builder/components-elements.js`
- `libs/builder/components-widgets.js`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Identify the bug in a builder component or widget.
- Modify the relevant file in libs/builder/components-*.js.
- Commit with a message referencing the fix.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.