# Lost and Found for Jira

> Also from the same developer: [Quick Diagrams for Jira](quick-diagrams.md) and [Quick Checklist for Jira](quick-checklist.md) (user guides, privacy policies and support).

A recycle bin for Jira Cloud. When an issue is deleted, a copy is kept so a Jira admin can read it and bring it back.

- [User guide](#user-guide)
- [Privacy policy](#privacy-policy)
- [Support](#support)

---

## User guide

### 1. Install
Install the app from the Atlassian Marketplace. Nothing else is needed: right after installing, the app starts copying your existing issues in the background, and from then on it copies every issue that is created or changed.

Open **Jira settings › Apps › Lost and Found**. The green box at the top says **Protection is on** when the first copy has finished.

### 2. Find a deleted issue
The **Deleted issues** tab lists everything that was deleted, newest first, with who deleted it, when, and how many days it will be kept.

- Search by key or summary, filter by project, or switch between *Waiting in bin*, *Already restored* and *Everything*.
- **Export list** gives you the rows as CSV text to copy into a spreadsheet.
- If one person deletes 10 or more issues within 10 minutes, a warning appears at the top. **Show them** lists exactly those issues.

### 3. Restore
Press **Open** to read the issue: description, comments, people, labels. Under **What comes back**, untick anything you do not want (comments, work logs, links, status), then press **Restore issue**. The issue is created at once; comments, work logs and links are then added in the background, and the result (including anything that could not be restored) is shown when it is done.

To restore several at once, tick them in the list and press **Restore selected**. Parents are restored first so their sub-tasks can be attached to them.

**What comes back:** summary, description, type, priority, labels, assignee, reporter, due date, components, versions, custom fields the project accepts, comments, work logs, links, status (when the workflow has a direct step to it), and sub-tasks under their restored parent.

**What cannot come back:**
- Attached files. Jira erases them with the issue. Their names are kept so you know what was there.
- The original key and change history. Jira never reuses a deleted key, so the restored issue gets a new key and a note with the old one.
- The original author on comments and work logs. Jira shows the app as the author, so the real person and time are written in the text.
- Issues from a deleted project.
- Issues with a security level the app is not allowed to read, and comments or work logs restricted to a role or group the app is not in. Jira does not show these to the app, so they cannot be copied. For such issues only the deletion itself is recorded.

**Restrictions are kept.** An issue with a security level is restored with the same level, or not at all. A restricted comment or work log is restored with the same restriction, or not at all. Nothing is ever restored open to more people than before. To protect restricted issues, add the app to the security level and give it the *Set issue security* permission.

**Good to know.** Restoring creates a normal new issue, so your Jira may send its usual notifications and run automation rules. Old @mentions are turned into plain text so people are not notified again, and the label `lost-and-found-restored` is added so your rules can skip restored issues.

**Who can use it.** Only Jira administrators. They see every deleted issue the app could copy, including restricted ones.

### 4. Deleted comments
The **Deleted comments** tab lists comments that were deleted from issues that still exist. **Put back** adds the comment to the issue again.

### 5. Settings
- **Keep deleted issues for:** 30, 90, 180 or 365 days. After that the copy is erased for good.
- **Projects to leave out:** from then on, issues in these projects are not copied and their deletions are not recorded. Items already in the bin stay until their keep time ends.
- **Display language:** each person's Jira language, English, or Japanese.

---

## Privacy policy

_Last updated: 2026-11-16_

**Lost and Found for Jira** ("the app") runs entirely on Atlassian Forge.

### What the app stores
- Copies of Jira issues from your site (fields, comments, work logs, link and attachment names), so that deleted issues can be restored.
- Atlassian account IDs that appear in those issues. Profile data (display names, email addresses, avatars) is **not** stored, also not inside user fields or @mentions; names are read live from Jira when they are shown.
- Other text that people wrote in issues and comments is copied as written, so it can contain personal data if your users typed it there.
- App settings and the status of the one-time copy of existing issues.

### Where it is stored
Only in Atlassian Forge hosted storage for your site. The app makes **no requests to servers outside Atlassian**. The vendor has no access to your data.

### How long it is kept
- Copies of deleted issues and comments are erased automatically after the keep time you choose (30 to 365 days), or when an admin erases them from the bin.
- Copies of existing issues are replaced whenever the issue changes, and removed when the issue is deleted and its keep time ends.
- When the app is uninstalled, Atlassian removes all app data according to Forge's data retention rules.

### Personal data reporting
Once a week the app reports the account IDs it holds to Atlassian's personal data reporting service, as Atlassian requires. When Atlassian reports an account as closed, the app removes that account ID from its list; Jira then shows that person as a former user wherever the ID appears.

### What is not collected
No analytics, no tracking, no advertising, no cookies set by the app. Nothing is sold or shared.

### Permissions the app asks for
| Permission | Why |
|---|---|
| `read:jira-work` | Copy issues and receive create, update and delete events |
| `write:jira-work` | Create the issue, comments, work logs and links when restoring |
| `read:jira-user` | Write the original author's name into restored comments and work logs. Names are not stored. |
| `storage:app` | Keep the copies in Atlassian-hosted storage |
| `report:personal-data` | Report the stored account IDs to Atlassian's personal data reporting service |

### Contact
Questions about privacy: **t.p.o.radiation@gmail.com**

---

## Support

Email **t.p.o.radiation@gmail.com** or open an issue in this repository. Replies are sent in English or Japanese, usually within two business days.

Please include your Jira site address, what you did, and what you expected to happen. Do not send passwords or API tokens.
