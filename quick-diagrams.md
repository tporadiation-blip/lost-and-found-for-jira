# Quick Diagrams for Jira

Turn text into diagrams on any Jira issue. Write Mermaid, or paste it from ChatGPT, Claude or Copilot, and see the diagram as you type.

- [User guide](#user-guide)
- [Privacy policy](#privacy-policy)
- [Support](#support)

---

## User guide

### 1. Open the panel
Open any issue. Click the **Apps** button under the issue title and choose **Diagrams**. Jira keeps the panel on that issue from then on.

### 2. Add a diagram
Click **Add diagram**. Give it a name if you like, then write the diagram text. The preview on the right updates as you type. Not sure where to start? Pick one of the templates: Flowchart, Sequence, States, Data model, Timeline (Gantt), Mind map, Classes or Pie chart.

Pasting from an AI assistant: copy the whole answer block, including the ```` ```mermaid ```` lines. The app removes the wrapper for you.

If the text has a mistake, a short message shows the line, and the last good preview stays visible.

Click **Save**. Each issue can hold up to 30 diagrams of up to 20,000 characters each.

### 3. View, download and change
- **Full screen** opens a large view with zoom (−, Fit, +).
- **Download SVG** and **Download PNG** save the picture.
- **Copy text** copies the Mermaid text.
- **Edit** and **Delete** are shown only to people who can edit the issue.

### 4. Mermaid in descriptions
If the issue description has a code block with the language **mermaid** (or one that clearly starts with a Mermaid diagram type), the panel shows it under **Found in the description**. Click **Save as diagram** to keep a copy in the panel.

### 5. Language and theme
The panel follows your Jira language (English or Japanese) and your light or dark theme.

Mermaid syntax reference: https://mermaid.js.org/intro/syntax-reference.html

---

## Privacy policy

_Last updated: 2026-11-17_

**Quick Diagrams for Jira** ("the app") runs entirely on Atlassian Forge and has no servers of its own.

### What the app stores
- For each diagram: its name, its Mermaid text and the time it was last saved.
- Nothing else. The app does not store account IDs, names, email addresses or any other profile data.

### Where it is stored
Diagrams are stored as **issue properties** on the Jira issue they belong to, inside your Atlassian site. They are protected by Jira's own permissions, appear in Jira's data exports, and are deleted when the issue is deleted.

### What the app reads
The issue description (to find Mermaid code blocks), the diagrams on the issue, and whether the current user may edit the issue. This happens in the user's browser, as that user, through Atlassian's own interfaces.

### What is not collected
No analytics, no tracking, no cookies, no data sent to any server outside Atlassian. Diagrams are drawn in the browser with the open-source Mermaid library bundled inside the app.

### Permissions the app asks for
- `read:jira-work`: read the description, the diagrams and the user's edit permission on the issue.
- `write:jira-work`: save, change or delete diagrams that a user creates. The app changes nothing else on an issue.

### Contact
Questions about privacy: **t.p.o.radiation@gmail.com**

---

## Support

Email **t.p.o.radiation@gmail.com**. Replies are sent in English or Japanese, usually within two business days.

Please include your Jira site address, what you did, and what you expected to happen. Do not send passwords or API tokens.
