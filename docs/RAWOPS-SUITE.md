# RawOps Suite: apis that carry business context

[Portfolio overview](../README.md) · [RawOps Suite](https://github.com/RawPowered/RawOps-Suite) · [Evidence scope](EVIDENCE.md)

![RawOps case: APIs that carry business context](../assets/rawops/section.svg)

RawOps Suite adds a detailed PHP/MySQL integration case: provider-backed discovery, contextual assistance, scheduled communication and the records that connect one step to the next.

**Status:** The archive includes 122 API source files, within a wider application and migration history. Source and historical screens are available for inspection. Provider connectivity and end-to-end execution have not been revalidated.

## 1. Prepare context before calling a model

The email drafting handler loads active catalog values, lead activity, recent sample context and active promotions. The chat handler includes product and account context. The design question is what the model needs to answer the task accurately and what the interface lets an agent review.

[Email handler](https://github.com/RawPowered/RawOps-Suite/blob/main/api/ai-email-composer.php) · [Chat handler](https://github.com/RawPowered/RawOps-Suite/blob/main/api/ai-chat-streamlined.php) · [Historical composer](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/evidence/GALLERY.md#assisted-email-composition--28-october-2025) · [Product and learning design](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/PRODUCT-LEARNING-DESIGN.md)

**Evidence boundary:** Prompt constraints, including avoiding invented promotions, express intent. They do not guarantee factual output. The assistant capture shows a welcome state; it is not a model-quality benchmark.

## 2. Separate workflow intent from queued delivery

Templates, conditions, delays, processing, provider callbacks and analytics form a traceable communication design. The sample workflow preserves lead-linked outreach without creating a physical request solely to start an email sequence.

[Email lifecycle design](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/ENGINEERING-CASE-NOTES.md#3-give-email-automation-an-operational-feedback-loop) · [Workflow processing](https://github.com/RawPowered/RawOps-Suite/blob/main/api/email-workflow-processor.php) · [Queue processing](https://github.com/RawPowered/RawOps-Suite/blob/main/api/email-queue-processor.php) · [Provider webhook](https://github.com/RawPowered/RawOps-Suite/blob/main/api/sendgrid-webhook.php) · [Sample separation](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/ENGINEERING-CASE-NOTES.md#1-keep-sample-outreach-separate-from-fulfillment-work)

**Evidence boundary:** Source shows the boundaries and handlers. It does not prove an authenticated callback sequence, delivery guarantee or duplicate-safe behavior for every endpoint. These need isolated acceptance evidence.

## 3. Reuse data with explicit owners and identifiers

The Places adapter caches provider results and tracks usage. Shared shortcodes read product fields for both lessons and email templates. Invoice and commission case notes explain persisted identifiers, transaction ownership and notifications after commit.

[Places and usage](https://github.com/RawPowered/RawOps-Suite/blob/main/api/google-places-proxy.php) · [Shared product rendering](https://github.com/RawPowered/RawOps-Suite/blob/main/required/shortcode-engine.php) · [Email rendering](https://github.com/RawPowered/RawOps-Suite/blob/main/required/email-template-renderer.php) · [Invoice integrity](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/ENGINEERING-CASE-NOTES.md#2-protect-the-invoice-and-commission-handoff) · [API source index](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/API-INDEX.md)

**Evidence boundary:** Each handler has its own security and failure behavior. The archive documents gaps and restoration dependencies; a shared data path does not establish a universal API contract.

## Discuss the work

Ask me to trace the data used in an assisted draft, or separate sample outreach intent from the fulfillment and provider-delivery records.

The [systems diagram](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/SYSTEMS-ORCHESTRATION.md) provides the wider context. The [feature walkthrough](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/FEATURE-WALKTHROUGH.md) and [capability catalog](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/CAPABILITY-CATALOG.md) cover the rest of the platform.

## Evidence and maintenance

The source project preserves partial history of a previously functional application. Its published gallery contains 11 genuine historical captures with opaque redactions. [Publication checks](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/PUBLICATION-REVIEW.md) cover syntax and secret scanning; business workflows were not executed by those checks. Review [security and privacy](https://github.com/RawPowered/RawOps-Suite/blob/main/docs/SECURITY-AND-PRIVACY.md) before considering restoration.

This case was added October 26, 2026. Project source and evidence remain authoritative in RawOps Suite. No live CRM records were changed and no flows were run for this portfolio update.
