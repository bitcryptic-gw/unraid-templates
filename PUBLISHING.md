# Publishing templates

This repository is registered with Unraid Community Applications (CA). **Every push to `main` is live in the CA store** — there is no draft state or staging.

## Rules

- Add or change a template **only when Gary explicitly asks**, naming this repo and the template. Do not publish on your own initiative.
- Run the lint workflow (`.github/workflows/lint-templates.yml`) before pushing. It must pass on every `*.xml`.
- Never mirror live-server configuration (tailnet names, host names, mounts, extra args) into a template. Use generic defaults and placeholders only.
- Do not change an existing template's `<Repository>`, `<TemplateURL>`, or `<Date>` as part of unrelated work.
- A dangling `<TemplateURL>` is **not** a bug to fix by publishing. See the guardrail in the agent rule files.
