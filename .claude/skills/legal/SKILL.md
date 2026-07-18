---
name: legal
description: "Review, enhance, and maintain the KCM Trade legal & compliance documentation in this repository. Use for any task touching the policy/agreement/disclosure markdown files — drafting a new document, reviewing an existing one, checking cross-references and consistency, updating dates/versions, or assessing whether the wording adequately protects Kohle Capital Markets Limited. Triggers: legal review, compliance check, policy, disclosure, agreement, terms, privacy, AML/KYC, risk disclosure, draft a policy, update a policy."
---

# /legal — KCM Trade Legal & Compliance Documentation

This skill governs the legal, regulatory, and compliance documents published under the **KCM Trade** brand by **Kohle Capital Markets Limited** (the "Company"). It exists to do three jobs, always in service of protecting the Company:

1. **Review** — audit a document (or the whole set) for legal exposure, internal consistency, regulatory alignment, and broken references.
2. **Enhance** — strengthen protective wording, close gaps, and improve clarity without changing the Company's legal position unless asked.
3. **Maintain** — keep dates, versions, cross-links, and the index accurate as documents change.

> **Scope boundary — read first.** These are template/informational compliance documents, not legal advice. This skill helps draft and maintain them to a high standard, but it does **not** replace review by qualified counsel or the Company's compliance officer. Flag anything that changes the Company's legal obligations or regulatory posture for human sign-off. Never invent regulatory facts (licence numbers, regulator names, statutory citations, fund-protection figures) — if a fact isn't already established in the repo, mark it `[VERIFY]` rather than guessing.

---

## 1. Company facts (the source of truth)

Use these exactly; do not vary the wording. If a document contradicts these, that is a finding.

| Fact | Value |
|---|---|
| Legal entity | **Kohle Capital Markets Limited** |
| Trading name | **KCM Trade** |
| Incorporation | Republic of Mauritius |
| Regulator | Financial Services Commission of Mauritius (FSC) |
| Service model | Execution-only access to leveraged / derivative financial instruments |
| Australia entity (separate) | **Kohle Capital Markets Pty Ltd**, AFSL 489437 — see `australia-disclosure.md`; never merge the two entities |
| Support email | CS@kcmtrade.com |
| Compliance/enquiries | it.th@kcmtrade.com |
| Site | https://www.kcmtrade.com |
| Published docs base | https://kcm-trade.github.io/kcmtrade-legal/ |
| Defined party terms | "the Company", "we", "us", "our"; user is "User", "you", "your" |

Any regulatory fact **not** in this table or already written into an existing, committed document must be treated as unverified — insert `[VERIFY: …]` and surface it, never fabricate.

---

## 2. Document conventions (house style)

Every published document is a Jekyll page. Match this exactly.

**Frontmatter** (required on every published `.md`):
```yaml
---
layout: default
title: <Human Readable Title>
effective_date: <e.g. 1 March 2018>
last_updated: <e.g. 18 July 2026>
---
```

**Structure & register:**
- Opening paragraph defines the document, the Services, and the Company using the standard defined terms.
- Numbered `## N. Section Heading` sections; `---` horizontal rule between major sections.
- Formal legal register. Introduce defined terms in bold + quotes on first use: **KCM Trade** brand (the "Services").
- British spelling (organise, summarise, licence as noun) — consistent with the existing corpus.
- State that documents are "read together" and "incorporated by reference" where relevant.

**Cross-references** — always use the Jekyll relative_url filter, never bare paths:
```liquid
[Terms of Service]({{ '/terms-of-service.html' | relative_url }})
```
External links open safely: `{:target="_blank" rel="noopener noreferrer"}`.

**Versioned agreement tables** (as in `terms-of-service.md`) use `| Document | Version |` with PDF links; bump the version column when the underlying PDF changes.

---

## 3. Review workflow

When asked to review a document (or "review the docs"):

1. **Read the target(s) in full.** For a set-wide review, start with `index.md`, `README.md`, `terms-of-service.md` (the hub), then the specific policy.
2. **Run the protection checklist (§4).** Report findings as concrete, located items — `file.md:section` → issue → suggested fix — ordered by legal exposure (highest first).
3. **Run the consistency checklist (§5).**
4. **Separate findings into two buckets:**
   - *Safe to apply* — typos, broken links, stale dates, wording clarity, missing standard clauses that already exist elsewhere in the corpus.
   - *Needs human sign-off* — anything that shifts the Company's liability, rights, regulatory representations, or client obligations. Present these; do not silently apply.
5. **Only edit after the split is clear.** When you do edit, bump `last_updated` (§6).

Do not report a wall of nitpicks. Lead with what actually exposes the Company.

---

## 4. Protection checklist (does the wording protect the Company?)

For each reviewed document, verify the Company is shielded where the law allows:

- **Risk & no-advice** — leveraged-product risk warnings present; execution-only stated; "nothing herein is investment advice" where relevant.
- **Limitation of liability** — losses, indirect/consequential damages, force majeure, third-party/technology failures, and market-data reliance are addressed and capped where lawful.
- **No warranty** — Services provided "as is"; uptime, accuracy, and fitness disclaimers present.
- **Indemnity** — User indemnifies the Company for misuse, breach, and unlawful use.
- **Right to amend / suspend / terminate** — Company reserves the right to modify documents (effective on publication), suspend accounts, and refuse/close relationships (AML, sanctions, appropriateness).
- **Jurisdiction & governing law** — governing law and dispute forum stated; jurisdictional availability / restricted-territories carve-outs consistent with `jurisdictional-availability.md` and `sanctions-policy.md`.
- **Regulatory accuracy** — FSC Mauritius status stated correctly; no over-claiming of protections; Australia entity kept distinct.
- **Data protection** — lawful basis, data subject rights, retention, cross-border transfer, and breach handling covered; consistent with `privacy-policy.md`, `cookie-policy.md`, `data-safety.md`.
- **AML/KYC/sanctions** — verification, monitoring, refusal, and reporting rights reserved; consistent across `aml-kyc-policy.md` and `sanctions-policy.md`.
- **Severability & entire agreement** — one clause invalid doesn't void the rest; the document set is the entire agreement.
- **App-store alignment** — where relevant, disclosures still satisfy Google Play Data Safety / Apple App Privacy expectations (`data-safety.md`, `app-access-disclosure.md`).

A missing item from this list on a document where it belongs is a finding, not a stylistic preference.

---

## 5. Consistency checklist (across the corpus)

- **Company facts** match §1 everywhere (entity name, regulator, jurisdiction, contacts).
- **Cross-links resolve** — every `{{ '/x.html' | relative_url }}` points to a real `x.md`. Check both directions: documents that should reference each other do.
- **Defined terms** are used consistently ("the Services", "the Company") and not redefined differently between files.
- **Dates are coherent** — `effective_date` ≤ `last_updated`; a document edited today has today's `last_updated`.
- **Version tables** in `terms-of-service.md` reflect the current PDFs.
- **Index & README** list every published document; no orphan files, no dead entries.
- **Australia separation** — AU-specific content lives only in `australia-disclosure.md` and names the Pty Ltd entity + AFSL.

---

## 6. Maintenance rules

- **Any substantive edit** to a document → set `last_updated` to today's date (currentDate from context; today is authoritative). Never touch `effective_date` unless the Company's obligations genuinely change from a new date.
- **New document** → create with full frontmatter, add it to `index.md` and `README.md`, and cross-link it from every related document (and back).
- **Renamed/removed document** → fix every inbound `relative_url` link, `index.md`, and `README.md`.
- **After changes**, re-run §5 to confirm nothing dangles.
- This repo also uses **graphify** — after edits, `graphify update .` keeps the knowledge graph current (per project CLAUDE.md).

---

## 7. Drafting a new document

1. Confirm the document's purpose and which existing documents it interacts with.
2. Start from the closest existing document as a structural template (don't start from a blank page — the corpus has a consistent voice).
3. Apply §2 conventions, §4 protective clauses appropriate to the document type, and §1 facts.
4. Mark every unverified regulatory fact `[VERIFY: …]`.
5. Wire it into `index.md`, `README.md`, and related documents.
6. Set `effective_date` and `last_updated`; flag for compliance-officer sign-off before it goes live.

---

## 8. Output discipline

- Findings are **located and actionable**: `file.md § N` → what's wrong → suggested wording.
- Rank by exposure to the Company, not by ease of fixing.
- Distinguish "I applied this" from "this needs your lawyer/compliance officer."
- When you change legal wording, quote the before/after so a human can review the delta.
- Never assert a regulatory fact you cannot trace to §1 or a committed document.
