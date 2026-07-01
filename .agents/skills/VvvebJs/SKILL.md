```markdown
# VvvebJs Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the core development patterns and workflows used in the VvvebJs JavaScript codebase. You'll learn the project's coding conventions, how to fix bugs in builder components, update UI layouts, and understand the structure of testing within the repository. This guide is ideal for contributors looking to quickly get up to speed with VvvebJs development practices.

## Coding Conventions

**File Naming**
- Uses camelCase for file names.
  - Example: `componentsElements.js`, `editorPanel.js`

**Import Style**
- Uses relative imports.
  - Example:
    ```javascript
    import { someFunction } from './utils/helpers.js';
    ```

**Export Style**
- Prefers named exports.
  - Example:
    ```javascript
    export function updatePanel() { ... }
    export const PANEL_TYPE = 'sidebar';
    ```

**Commit Messages**
- Freeform style, often referencing the change directly.
  - Example: `fix video mute in widgets`
  - Average length: ~26 characters

## Workflows

### Fix Bug in Component or Widget
**Trigger:** When you need to fix a bug in a builder component or widget (e.g., video mute issue).
**Command:** `/fix-component-bug`

1. Identify the bug in a builder component or widget.
2. Locate and modify the relevant file, typically in `libs/builder/components-elements.js` or `libs/builder/components-widgets.js`.
3. Commit your changes with a message referencing the fix.

**Example:**
```javascript
// libs/builder/components-widgets.js
export function fixVideoMute() {
  // Bug fix implementation
}
```
Commit message: `fix video mute in widgets`

---

### Update UI Layout or Panels
**Trigger:** When you want to change the layout or move UI panels (e.g., moving tabs to sidebar).
**Command:** `/update-ui-layout`

1. Edit the relevant CSS and SCSS files to reflect UI changes:
    - `css/editor.css`
    - `scss/_builder.scss`
    - `scss/editor.scss`
2. Commit your changes with a message describing the UI update.

**Example:**
```scss
// scss/editor.scss
.sidebar-tabs {
  display: flex;
  flex-direction: column;
}
```
Commit message: `move tabs to sidebar in editor`

## Testing Patterns

- **Framework:** Unknown (not detected)
- **Test File Pattern:** Files matching `*.test.*`
  - Example: `component.test.js`
- Tests are likely colocated with source files or in dedicated test directories.

## Commands

| Command              | Purpose                                                   |
|----------------------|-----------------------------------------------------------|
| /fix-component-bug   | Fix a bug in a builder component or widget                |
| /update-ui-layout    | Update the UI layout or move panels/tabs in the interface |

```