# Backupify (backupify)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Backupify (by Datto/Kaseya) is a SaaS backup platform providing automated cloud-to-cloud data protection for Google Workspace and Microsoft 365. It offers seat-level backup coverage for users, shared mailboxes, SharePoint sites, team sites, and Microsoft Teams. The SaaS Protection REST API enables MSPs and enterprise IT teams to automate domain administration and seat licensing programmatically.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - SaaS Backup, Data Protection, Cloud Backup, Microsoft 365, Google Workspace

## Timestamps

- **Created:** 2026-03-27
- **Modified:** 2026-04-19

## APIs

### Backupify SaaS Protection API
The Backupify SaaS Protection REST API enables programmatic management of cloud-to-cloud backup for Microsoft 365 and Google Workspace. Covers domain listing, seat enumeration, and bulk seat licensing operations. Authentication uses HTTP Basic auth with API key credentials.

**Human URL:** [https://www.backupify.com/](https://www.backupify.com/)

#### Tags:

 - SaaS Backup, Data Protection, Microsoft 365, Google Workspace

#### Properties

- [Documentation](https://saasprotection.datto.com/help/M365/Content/Other_Administrative_Tasks/using-rest-api-saas-protection.htm)
- [OpenAPI](openapi/backupify-saas-protection-api.yaml)

## Common Properties

- [Website](https://www.backupify.com)
- [Documentation](https://saasprotection.datto.com/help/M365/Content/Other_Administrative_Tasks/using-rest-api-saas-protection.htm)
- [Portal](https://portal.dattobackup.com)
- [Pricing](https://www.backupify.com/pricing)
- [Blog](https://www.datto.com/blog/)
- [Support](https://www.datto.com/support/)
- [TermsOfService](https://www.datto.com/legal/terms-and-conditions/)
- [PrivacyPolicy](https://www.datto.com/legal/privacy-policy/)
- [GitHubOrganization](https://github.com/backupify)

## Features

| Name | Description |
|------|-------------|
| Microsoft 365 Backup | Automated cloud-to-cloud backup for Exchange, OneDrive, SharePoint, and Teams. |
| Google Workspace Backup | Automated backup for Gmail, Drive, Contacts, and Calendar. |
| Seat-Level Control | License, unlicense, or pause backup at the individual user, mailbox, site, or team level. |
| Bulk Seat Management | Manage up to 100 seat changes in a single API call. |
| MSP Multi-Tenant | Manage backup across multiple customer domains from a single pane of glass. |
| Point-in-Time Recovery | Restore data to any point in time with granular item-level recovery. |

## Use Cases

| Name | Description |
|------|-------------|
| SaaS Data Protection | Protect Microsoft 365 and Google Workspace data from accidental deletion, ransomware, and insider threats. |
| MSP Backup Management | Automate backup seat provisioning and de-provisioning across multiple customer tenants. |
| Compliance and Archival | Maintain immutable backups for compliance, legal hold, and audit requirements. |
| Migration Support | Backup source data before and during cloud-to-cloud migrations. |

## Integrations

| Name | Description |
|------|-------------|
| Microsoft 365 | Native integration with Exchange Online, OneDrive, SharePoint, and Microsoft Teams. |
| Google Workspace | Native integration with Gmail, Google Drive, Contacts, and Calendar. |
| Kaseya VSA | Integration with Kaseya RMM for MSP workflow automation. |
| Datto RMM | Integration with Datto RMM for endpoint and SaaS backup orchestration. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Backupify SaaS Protection API](openapi/backupify-saas-protection-api.yaml)

### JSON Schema

- [Domain](json-schema/saas-protection-api-domain-schema.json)
- [Seat](json-schema/saas-protection-api-seat-schema.json)
- [BulkSeatChangeRequest](json-schema/saas-protection-api-bulk-seat-change-request-schema.json)
- [+ 5 more schemas](json-schema/)

### JSON-LD

- [Backupify JSON-LD Context](json-ld/backupify-context.jsonld)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Backupify SaaS Protection API](capabilities/shared/saas-protection-api.yaml) — 3 operations for domain listing, seat listing, and bulk seat management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [SaaS Backup Management](capabilities/saas-backup-management.yaml) | SaaS Protection API | 3 | MSP Technician, IT Administrator |

## Vocabulary

- [Backupify Vocabulary](vocabulary/backupify-vocabulary.yaml) — Unified taxonomy mapping 2 resources, 4 actions, 1 workflow, and 2 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Backupify Spectral Rules](rules/backupify-spectral-rules.yml) — 12 rules across 5 categories enforcing Backupify API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
