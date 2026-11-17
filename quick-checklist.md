# Quick Checklist for Jira

A simple checklist on every Jira issue. Paste a list from anywhere, tick items off, and find unfinished checklists with JQL.

- [User guide](#user-guide)
- [Privacy policy](#privacy-policy)
- [Support](#support)

---

## User guide

### 1. Open the panel
Open any issue. Click the **Apps** button under the issue title and choose **Checklist**. Jira keeps the panel on that issue from then on.

### 2. Add items
Type an item and press **Enter**. To add many at once, paste a list: one item per line. Bullets (`-`, `*`, `1.`) and task lists (`- [ ] item`, `- [x] item`) as written by ChatGPT, Claude or Copilot are understood. Headings and code fences are skipped.

New to checklists? Start from a template: Definition of done, Bug fix, Release or Onboarding.

A checklist holds up to 100 items of up to 200 characters each.

### 3. Work through it
- Tick an item when it is done. The progress bar shows how far along you are.
- Hover over an item to move it up or down, edit it (or double-click the text), or delete it.
- **Hide done** keeps long lists short. **More** lets you copy the list as text, remove done items, or delete the checklist.
- Edit and delete are shown only to people who can edit the issue.

If two people change the same checklist at the same moment, the app does not overwrite the other person's change: it reloads the newer list and asks you to try again.

### 4. Find issues with JQL
Each issue's checklist counts are searchable:
- `checklistOpen > 0` — issues with unfinished items
- `checklistComplete = yes` — issues whose checklist is fully done
- `checklistTotal`, `checklistDone` — number of items and done items

### 5. Language and theme
The panel follows your Jira language (English or Japanese) and your light or dark theme.

---

## Privacy policy

_Last updated: 2026-11-17_

**Quick Checklist for Jira** ("the app") runs entirely on Atlassian Forge and has no servers of its own.

### What the app stores
- For each issue: the checklist item texts, whether each item is done, the item counts, and the time of the last save.
- Nothing else. The app does not store account IDs, names, email addresses or any other profile data.

### Where it is stored
The checklist is stored as an **issue property** on the Jira issue it belongs to, inside your Atlassian site. It is protected by Jira's own permissions, appears in Jira's data exports, and is deleted when the issue is deleted.

### What the app reads
The checklist on the issue and whether the current user may edit the issue. This happens in the user's browser, as that user, through Atlassian's own interfaces.

### What is not collected
No analytics, no tracking, no cookies, no data sent to any server outside Atlassian.

### Permissions the app asks for
- `read:jira-work`: read the checklist and the user's edit permission on the issue.
- `write:jira-work`: save the checklist that a user changes. The app changes nothing else on an issue.

### Contact
Questions about privacy: **t.p.o.radiation@gmail.com**

---

## Support

Email **t.p.o.radiation@gmail.com**. Replies are sent in English or Japanese, usually within two business days.

Please include your Jira site address, what you did, and what you expected to happen. Do not send passwords or API tokens.
