# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links
- The Guides tab is user-facing product documentation; the API reference tab is maintained separately — do not modify it when working on Guides

## Terminology

- Use "workspace" for the tenant a user works in; the UI also calls it a "company" — prefer "workspace" in prose and use "company" only when quoting UI labels such as **Create a company**
- A "member" belongs to a workspace; a "guest" only sees pages shared with them — don't write "user" when "member" or "guest" is meant
- "Programs" (capitalized) is the sidebar section that holds the workspace's pages
- A "page" is a block-based screen; a "block" is a unit inside a page (Table, Page, Callout, Report, Operation, Dashboard)
- A "table" holds "records"; records have "fields"; tables display through "views" (Table, Board, Calendar, Gallery, Dashboard)
- A "form" is the record editor; a "form template" is a saved, reusable form layout edited in the Page Designer
- A "workflow" is a visual automation built in **Workflows**; a "field rule" is logic attached to form events in the Page Designer — never conflate the two
- A "stakeholder" is the shared master record for people and companies (customers, suppliers, employees, drivers, insurers)
- Spanish terms appear in parentheses only where they help Colombian users recognize a concept: causación, remisión, NIT, DIAN, RNDC

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Text-first: no screenshots or image paths unless a current, accurate asset exists in `/images`
- Use absolute internal links, for example `/data/tables`

## Content boundaries

Guides document only verified, generally available product behavior. Do not document:

- Budgeting — no user-facing capability exists
- Health/clinical records — no user-facing surface in the current product
- Customer-specific verticals — not part of the general product
- The legacy workflow screen — superseded by **Workflows**
- The video-agents ("Employees") gallery — not user-ready
- The Relation view type — non-functional
- Knowledge sync settings — not generally available; describe Agent Tasks as import tracking only
- Company ownership hierarchies — not yet released
- API endpoints, request formats, authentication headers, schemas, or SDK usage — the API reference tab covers developers; Guides may mention API keys only as a workspace setting
- Internal implementation details: framework class names, database tables, endpoint paths, identifiers, environment variables, secrets
