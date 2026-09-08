# Strategos Telos — Site Governance

**Project owner:** Tobias Malan
**Site URL:** https://TobiasDraven.github.io/strategostelos-wiki/
**Repository:** https://github.com/TobiasDraven/strategostelos-wiki
**Effective:** 2026-09-06
**Status:** Ratified — awaiting agent identity resolution

---

## Purpose

Strategos Telos is a curated knowledge base for military theory, wargaming, scenario design, and strategic analysis. It exists to serve the SANDF and broader defence community with rigorously sourced, properly attributed content.

## Content Diversity Principle

For every one "Western" thing on this site — be it a concept, page, article, example, or case study — there must be **two more**:

1. **An African perspective** — grounded in Sub-Saharan Africa specifically, with attention to the continent's diversity (not reducing Africa to a monolith).
2. **A perspective from Asia, South America, or another "developing" part of the world** — ensuring the site reflects the majority of the world's population and military experience.

This **2:1 ratio** is a guiding principle. It applies to:
- Case studies (e.g., one Western battle → one African battle → one Asian/South American battle)
- Examples and scenarios
- Historical narratives
- Theoretical frameworks (e.g., one Western theorist → one African theorist → one Asian theorist)
- Training manual procedures (adaptable to different resource environments)

**Within Africa:** Sub-Saharan Africa is the primary focus. North African perspectives are included where relevant but do not substitute for Sub-Saharan representation.

**Why:** Military knowledge has been overwhelmingly written from a Western perspective. This site corrects that imbalance. A military officer from Ghana, Vietnam, or Bolivia should see their experience reflected here — not as an afterthought, but as a core part of the catalogue.

**Implementation:** When proposing or writing a content piece, the author must identify the "two non-Western counterparts" that will accompany it. If they do not yet exist, they are flagged as pending.

1. **All substantive claims must cite their source.** No unattributed assertions.
2. **NO SANDF DOCTRINE.** No internal SANDF doctrine, no documents marked RESTRICTED, no confidential or classified material of any kind.
3. **Publicly available = fair game.** Information available on the internet may be used. Foreign military doctrine is permitted.
4. **Human-approved exceptions only.** If Tobias explicitly provides a document for wiki content, it is pre-approved — this does not create a precedent for future SANDF-internal documents.
5. **Attribution preserved.** Source documents are cited by title, reference number, and author where applicable.
6. **Draft → Review → Deploy.** No content reaches the live site without review.

## Agent Roles

| Agent | Role | Authority |
|-------|------|-----------|
| **Archon Telos (Hermes)** | Main writer, content curation, wiki architecture, quality control, deploy execution | Can write and deploy. Cannot approve own content. |
| **Apex (OpenClaw)** | Main writer, research, drafting, content review, governance enforcement | Can write and review. Cannot approve own content. |
| **Archon Atlas** | Main writer, worldbuilding, creative content, scenario design, narrative architecture | Can write and review. Cannot approve own content. |

## Identity Resolution

**Confirmed:** 2026-09-06

| Role | Agent Name | Inbox |
|------|-----------|-------|
| Hermes instance | ARCHON-TELOS | POST/OPEN/ARCHON TELOS/ |
| OpenClaw instance | APEX | POST/OPEN/APEX/ |
| Archon Atlas | ATLAS | POST/OPEN/ARCHON ATLAS/ |

All three agents are **main writers**. All three participate in peer review.

## Deploy Authority

- **Sunday deploy:** Content may be deployed only when **all three agents** (Archon Telos, Apex, Archon Atlas) have approved it.
- **Self-approval is forbidden.** An agent's own content must be reviewed and approved by at least one other agent.
- **Tobias retains final authority** on all content, structure, and governance decisions. Tobias may override any agent decision.

## OPSEC Rules (Hard Limits)

1. **No SANDF internal doctrine** — no exceptions beyond pre-approved documents explicitly provided by Tobias
2. **No RESTRICTED documents** — any document marked RESTRICTED, CONFIDENTIAL, or similar in body text or metadata is excluded
3. **No personal information** — no service numbers, names of personnel not already public, unit-level operational details
4. **No operational plans or procedures** — no COAs, OOBs, or deployment schedules
5. **When in doubt, ask Tobias** — ambiguity resolves to exclusion

## Workflow

```
Daily (Mon-Sat, ~0230 cron):
  - Check postbox for coordination messages
  - Check project folder for drafts and staging content
  - Research, write new content, review other agents' drafts
  - Send/receive coordination messages via postbox
  - Update project folder
  - Log cycle outcome

Sunday (publish day):
  - Review all staged content in content/
  - Confirm all three agents have approved each page
  - Verify OPSEC compliance
  - Deploy approved content to GitHub Pages
  - Log deployment in deploy-log/
  - Move deployed content to archive/

Maintenance (any day):
  - Critical fixes, broken links, navigation updates
  - Does not require full 3-agent approval if fixing factual errors in already-approved content
  - Log all maintenance in deploy-log/
```

## File Structure

```
GH-PAGES/STRATEGOS-TELOS/
├── governance/
│   └── SITE-GOVERNANCE.md    # This file
├── content/                  # Approved content pending deploy
├── drafts/                   # Work in progress
│   ├── ARCHON-TELOS/
│   ├── APEX/
│   └── ATLAS/
├── archive/                  # Deployed content snapshots
├── deploy-log/               # Deployment records
├── WORKFLOW.md               # Agent workflow specification
└── README.md                 # Project overview
```

## Site Structure Guidelines

- **Depth:** Keep navigation trees to **4–6 levels** max, with **4 as the preferred target**.
- **Sidebar:** Minimalist but functional. Sections stay collapsed by default until the user opts in.
- **Discoverability:** Core resources and frequently used pages should be reachable within **1–2 clicks** from Home.
- **Modularity:** Prefer multiple focused pages over one long page. This keeps edits small, review simple, and nav usable.
- **Search:** The site includes built-in visitor search via the MkDocs Material search plugin. Users can search page titles and content directly from the search bar.

## Site Structure

- **Authoritative working copy:** `C:\Users\malan\strategostelos-wiki`
- **Project org folder:** `C:\OBSIDIAN-VAULT\ASTRALIS\GH-PAGES\STRATEGOS-TELOS`
- These two locations must stay in sync. When one is updated, update the other.

## Site Purpose

Strategos Telos operates as two integrated resources in one:

### 1. Encyclopedia

Reference entries that define concepts, frameworks, history, and terminology. These pages are:
- **Definitive:** meant to be authoritative and stable
- **Cited:** every substantive claim links to a source
- **Neutral in tone:** descriptive, not prescriptive
- **Cross-linked:** related concepts connect via internal links
- **Long-lived:** updated when understanding evolves, not rewritten for style

### 2. Universal Training Manual

Progressive, applied guidance for practitioners. These pages are:
- **Actionable:** step-by-step procedures, checklists, templates, and examples
- **Modular:** focused pages that can be read alone or as part of a sequence
- **Practical:** designed for use during planning, execution, or instruction
- **Evolving:** improved as new methods and feedback emerge

### How They Work Together

- Encyclopedia pages explain **what** something is and **why** it matters.
- Training manual pages explain **how** to apply it.
- A student should be able to start at either side and find the other through cross-reference.

## Site Structure Guidelines

- **Depth:** Keep navigation trees to **4–6 levels** max, with **4 as the preferred target**.
- **Sidebar:** Minimalist but functional. Sections stay collapsed by default until the user opts in.
- **Discoverability:** Core resources and frequently used pages should be reachable within **1–2 clicks** from Home.
- **Modularity:** Prefer multiple focused pages over one long page. This keeps edits small, review simple, and nav usable.
- **Search:** The site includes built-in visitor search via the MkDocs Material search plugin. Users can search page titles and content directly from the search bar.

## Writing Standards

### Encyclopedia-style pages
- Start with a clear definition or summary.
- Use headings to break concepts into scannable sections.
- Include a “See also” or cross-reference block where relevant.
- Cite sources for factual claims.

### Training manual-style pages
- Start with a concise purpose statement or learning objective.
- Use numbered steps, tables, and checklists.
- Include examples, templates, or worked problems where possible.
- Keep procedures testable: a reader should be able to act on the page without additional context.

## Security

1. **Public repository** — all content is publicly accessible
2. **No credentials, tokens, or keys** in any content file
3. **Content review is mandatory** before deploy
4. **Governance violations** are reported to Tobias immediately via postbox
5. **OPSEC violations** result in immediate content removal and incident report to Tobias

## Escalation

Agents cannot resolve a dispute → escalate to Tobias via postbox (`POST/OPEN/TOBIAS/`).

## Identity Resolution

Pending. The three agents must resolve canonical names among themselves before the first Sunday deploy. Proposed scheme:
- `ARCHON-TELOS` or `TELOS` — Hermes instance
- `APEX` — OpenClaw instance  
- `ATLAS` — Archon Atlas

Agents confirm or propose alternatives via postbox.

## Ratification

| Decision | Value |
|----------|-------|
| Deploy gate | 3-agent peer review, all must approve |
| OPSEC | No SANDF doctrine. Public info only. |
| Cron | Daily ~0230, Sunday deploy |
| Roles | All three agents are main writers |
| First deploy | 2026-09-13 |

---

*Sisyphus is happy. The wiki is governed anyway.*
