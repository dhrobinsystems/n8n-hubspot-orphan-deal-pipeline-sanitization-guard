# ⚠️ Disclaimer & Liability Limitation

**Use at your own risk.** The code, workflows, and scripts in this repository (`n8n-hubspot-orphan-deal-pipeline-sanitization-guard`) are provided for educational and architectural demonstration purposes.

## No Liability

The author and dhRobin Systems accept no responsibility or liability for any direct, indirect, incidental, or consequential damages that result from using, misusing, or deploying these scripts. This includes, without limitation, lost revenue, inaccurate forecasts or pipeline reports, deals moved to an unintended stage, overwritten or cleared property values, duplicate or misassigned tasks, unintended disclosure of deal or customer information, service interruptions, and API quota exhaustion.

## No Warranty

All software, n8n JSON blueprints, JavaScript modules and prompts are provided "AS IS", without warranty of any kind, express or implied. This includes, but is not limited to, warranties of merchantability, fitness for a particular purpose, and non-infringement.

No warranty is given that the audit detects every non-compliant deal; that association, property, stage or activity data returned by HubSpot is complete or current; that severity, quarantine, flag, clear or restore decisions are correct for your business; or that the circuit breaker will prevent every unintended change.

## Production Testing Required

Always test thoroughly in an isolated staging environment, such as a HubSpot developer test account or sandbox, with `SANDBOX_MODE=true`, `DRY_RUN=true` and `SYNC_TO_HUBSPOT=false` enabled, before you connect live HubSpot credentials. Enable property writes, remediation tasks, stage-mode quarantine, automatic restore and Slack notifications one step at a time, reviewing the output of each step before the next. Keep conservative circuit-breaker limits in production.

Treat every quarantine decision, stage move and remediation task as an automated recommendation that a person must review before it's relied on for forecasting or pipeline reporting.

## Third-Party APIs & Compliance

You alone are responsible for complying with the terms of service, rate limits, data privacy regulations (GDPR/CCPA), and security policies of HubSpot, Slack and any connected services. That includes:

- agreeing the hygiene rules, severities and quarantine behaviour with the sales and RevOps stakeholders whose pipelines they affect;
- making sure forecast, commission and board reports treat quarantined deals as intended;
- posting digests only to internal, access-controlled channels, because deal names and amounts can identify customers;
- preserving CRM property history and any audit records your organisation requires;
- securing, rotating and restricting access to the HubSpot private app token and the Slack webhook URL;
- reviewing every automatically created or updated record.

## No Affiliation

HubSpot, Slack and n8n are trademarks of their respective owners. This project is independent and is not affiliated with, endorsed by, or sponsored by any of them. All companies, deals, identifiers, pipelines and figures in the fixtures and pinned data are fictitious.

## Not Professional Advice

Nothing in this repository constitutes legal, privacy, security, accounting, or financial advice. Consult qualified professionals for your specific circumstances.

---

Released under the MIT License. Copyright (c) 2026 DH Robin (dhRobin Systems). See [LICENSE](LICENSE).

Full text: DISCLAIMER.md · Licensed under the MIT License. License: MIT © 2026 dhRobin Systems · Provided as-is, see the disclaimer.
