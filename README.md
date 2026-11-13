# DukaVault AI

**Private Business Intelligence Assistant for UGREEN AI NAS**  
UGREEN AI NAS Hackathon 2026 · Track: Automate Your Workflow · Entry: Individual / Solo

DukaVault AI helps small-business owners review business records stored on an authorized UGREEN AI NAS. It is designed to find relevant documents, extract supported facts, compare related records, and produce concise summaries that link important findings back to their source files.

## The problem

Invoices, receipts, purchase records, inventory sheets, and supplier documents are often spread across folders. Manually comparing them takes time and makes it easy to miss price changes, duplicate records, missing evidence, or conflicting information.

## Proposed workflow

1. **Choose scope** — the user selects an authorized folder, time period, and business question.
2. **Find records** — discover relevant files within that authorized scope.
3. **Extract facts** — read supported documents and capture relevant details.
4. **Reconcile** — compare related records and identify confirmed differences, possible duplicates, and missing evidence.
5. **Report with evidence** — return a concise summary with source-file references, uncertainty labels, and limitations.

## Example questions

- Why did supplier costs increase this month?
- Which invoice prices changed compared with the previous period?
- Are there possible duplicate supplier invoices?
- Which purchase records are missing supporting documents?

## Design principles

- **Evidence first:** material findings should point to their source files.
- **Human control:** the initial design is read-only; no autonomous file changes.
- **Privacy and scope:** process only files the user has authorized.
- **Honest uncertainty:** distinguish confirmed differences from possible issues or unreadable evidence.
- **Safe document handling:** treat file contents as untrusted data, not as instructions to the agent.

## Project status

This repository contains the proposal, workflow documentation, draft Skill instructions, and submission video script.

**Current stage: proposal / initial Skill package preparation.** The package still needs to be imported and checked with the official UGREEN UGOS Skill Creation Tool, mapped to the exact agents and capabilities registered in the target environment, and validated on a UGREEN AI NAS. No live NAS runtime test or production integration is claimed.

See:
- [Hackathon proposal](docs/UGREEN_HACKATHON_PROPOSAL.md)
- [Draft Skill instructions](SKILL.md)
- [Validation checklist](docs/VALIDATION.md)
- [Submission video script](docs/VIDEO_SCRIPT.md)

## Limitations

Results depend on supported document formats, readable source files, extraction quality, and capabilities available in the installed UGREEN tool version. DukaVault AI is not accounting software, does not determine fraud, and does not make autonomous changes to business files.

## Third-party components

No third-party components are included in this initial documentation package. UGREEN UGOS and the official UGREEN Skill Creation Tool are the intended host platform and development tools.
