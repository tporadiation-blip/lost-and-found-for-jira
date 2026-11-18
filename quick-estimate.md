# Quick Estimate: Planning Poker for Jira

Planning poker on every Jira issue. Everyone picks a card, cards stay hidden until the reveal, and the agreed estimate goes straight into Story Points.

- [User guide](#user-guide)
- [Privacy policy](#privacy-policy)
- [Support](#support)

---

## User guide

### 1. Open the panel
Open any issue. Click the **Apps** button under the issue title and choose **Estimate**. Jira keeps the panel on that issue from then on.

### 2. Pick your card
Click a card. You can change it, or click it again to take it back, until the cards are revealed. Other people see only that you have voted, never your card. **?** means "not sure" and **☕** means "I need a break"; neither is used in the numbers.

Your team does not need to be in a meeting: people can vote at different times. The panel checks for new votes every few seconds while it is open.

### 3. Reveal and agree
People who can edit the issue see **Reveal cards**. After the reveal everyone sees each card, the average, the median, the range and how the votes are spread. If the votes are two or more cards apart, the panel suggests talking it through and voting again.

Click **Agree on …** (the suggestion is the smallest card not below the median) or pick another value. If the issue has a Story Points or Story point estimate field, **Set Story Points to …** writes the agreed value into it.

### 4. New round and decks
**New round** clears all cards. Decks: Fibonacci, Modified Fibonacci, Powers of 2 and T-shirt sizes. Changing the deck starts a new round.

### 5. Who can do what
- People who can view the issue can vote and see the result after the reveal.
- People who can edit the issue can also reveal, start a new round, agree on an estimate and set Story Points.
- Jira checks these permissions on the server for every action.

### 6. Language and theme
The panel follows your Jira language (English or Japanese) and your light or dark theme.

---

## Privacy policy

_Last updated: 2026-11-18_

**Quick Estimate: Planning Poker for Jira** ("the app") runs entirely on Atlassian Forge and has no servers of its own.

### What the app stores
- For each issue: the round number, the deck, whether the cards have been revealed, and the agreed value.
- For each vote: the voter's Atlassian account ID and the card. The app does not store names, email addresses or avatars.
- A list of the account IDs it holds, used only for Atlassian's personal data reporting.

### Where it is stored and for how long
In the app's own Forge storage on Atlassian. Cards are deleted when a new round starts and when the issue is deleted, and automatically after 90 days at the latest. When Atlassian reports that an account has been closed, the app deletes that account's cards and its ID.

### What the app reads
Whether the current user may view and edit the issue (checked on the server, as that user), the names and avatars of the people who voted (read in the viewer's browser and shown, not stored), and the issue's edit screen to find a Story Points field.

### What the app writes
Only the Story Points field, and only when a user clicks **Set Story Points**.

### What is not collected
No analytics, no tracking, no cookies, no data sent to any server outside Atlassian.

### Permissions the app asks for
- `read:jira-work`: check the user's permissions on the issue and find the Story Points field.
- `write:jira-work`: set Story Points when a user asks for it.
- `read:jira-user`: show the names and avatars of the people who voted.
- `storage:app`: keep the cards hidden until the reveal.
- `report:personal-data`: report the stored account IDs to Atlassian so that closed accounts are removed.

### Contact
Questions about privacy: **t.p.o.radiation@gmail.com**

---

## Support

Email **t.p.o.radiation@gmail.com**. Replies are sent in English or Japanese, usually within two business days.

Please include your Jira site address, what you did, and what you expected to happen. Do not send passwords or API tokens.
