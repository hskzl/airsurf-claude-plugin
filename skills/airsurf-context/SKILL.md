---
name: airsurf-context
description: Pull the brief, decisions and open issues of an Airsurf project or issue before working on it. Use when the person names an Airsurf issue key (like WEB-12), a project, or asks to "work on" something tracked in Airsurf.
---

# Load the context from Airsurf first

Before writing code for tracked work, read what the team already decided, so the change matches it.

1. Find the item: an issue key goes to `get_issue`; a name goes to `search`.
2. Read it in full with `read`, then call `get_related` to see the pages, designs, issues and events linked to it.
3. Read the linked brief or spec pages that matter. Note decisions, constraints and open questions.
4. Tell the person in a few lines what you found (with links) before you start, and point out any conflict between the request and a recorded decision.
5. When you start a branch, use `get_branch_name` for the issue. When a pull request exists, link it with `link_pull_request`.
