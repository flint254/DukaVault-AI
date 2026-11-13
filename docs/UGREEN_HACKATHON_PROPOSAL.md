# DukaVault AI — UGREEN AI NAS Hackathon 2026

**Project:** DukaVault AI  
**Description:** Private Business Intelligence Assistant  
**Track:** Automate Your Workflow  
**Entry:** Individual / Solo

## 1. What does the Skill do?

DukaVault AI reviews authorized business documents on UGREEN AI NAS, reconciles related records, and produces evidence-backed summaries of business changes.

## 2. Target user and problem

Small-business owners and administrators often keep invoices, purchase records, inventory documents, and supplier files in separate folders. Finding changes or conflicting information manually is slow and error-prone.

## 3. Proposed solution

The Skill discovers relevant authorized files, reads supported documents, extracts key facts, compares records, and reports confirmed differences, possible duplicates, and missing evidence with source references.

## 4. Core user flow

The user selects an authorized folder, period, and question. The Skill finds relevant records, reads them, reconciles related facts, validates material findings against sources, and returns a concise report with evidence and limitations.

## 5. Difference from existing tools

Rather than offering generic document chat, DukaVault follows an evidence-first reconciliation workflow: every material finding is tied to the original NAS file, uncertainty is labelled, and missing evidence is kept distinct from confirmed discrepancies.

## 6. UGREEN AI NAS capabilities

The intended workflow uses supported file discovery/browsing to locate records, document reading and extraction to understand them, and supported document/knowledge lookup or reconciliation to compare results. Only capabilities exposed by the official Skill Creation Tool will be invoked.

## 7. Technical approach

The Skill is intended to orchestrate registered UGREEN expert agents by capability: file discovery, document extraction, and cross-record reconciliation. Each stage should pass forward actual file references and results. It must respect user-authorized scope, treat file contents as untrusted data, and remain read-only unless the user explicitly confirms a supported change. No custom scripts or unsupported CLI commands are assumed.

## 8. Development status

The initial Skill instructions, user flow, reporting format, privacy boundaries, and validation guidance are prepared. Importing and checking the package with the official UGOS Skill Creation Tool, mapping its exact registered agents/capabilities, and NAS runtime validation remain pending.

## 9. Final validation plan

- **Core test 1:** Compare two supplier invoices and verify each reported difference against the original files.
- **Core test 2:** Review a month of purchase records and produce a sourced change summary.
- **Edge case:** Unreadable or conflicting documents must be flagged as uncertain without invented values.

## 10. Limitations and dependencies

Results depend on supported document formats, readable source files, accurate extraction, and the capabilities available in the installed UGREEN tool version. The Skill does not replace accounting software, determine fraud, or perform autonomous file changes. NAS validation is pending.

---

**Disclosure:** This is an initial proposal-stage package. No UGREEN NAS runtime testing is claimed. The Skill must be checked with the official UGOS Skill Creation Tool before submission.

**Third-party components:** None included in this initial package. UGREEN UGOS / UGREEN Skill Creation Tool are the required host platform and developer tools.
