# Agent instructions

## Pull request task tracking

Before implementing any repository task the user assigns, record it in the relevant pull request's description checklist, even if the user did not name a PR or frame the request as PR work. If multiple PRs are affected, add the task to each relevant PR. For repository work not yet associated with a PR, identify or create the intended PR before implementation. This applies to code and documentation work; read-only research and conversational tasks do not require a PR unless they lead to repository changes. Keep checklist status accurate as work progresses; mark an item complete only after its result is verified.

## User-facing copy

Do not add or change any text shown to product users without the user's explicit approval. This includes labels, helper text, tooltips, placeholders, warnings, notices, confirmation prompts, and error or success messages. Do not invent explanatory or safety copy as an implementation detail. If new copy seems necessary, propose the exact text and get approval before adding it. Existing copy may be changed only when the user explicitly requests that change.

## Production and Cloudflare changes

- Never deploy, publish, promote, or otherwise change production resources or production behavior without fresh, explicit written approval from the user that names the target and action. General requests to finish, release, or deploy do not override this requirement.
- Before adding or enabling a Cloudflare product, service, binding, storage resource, or other potentially billable platform capability, explain why it is needed and get the user's explicit approval. Prefer services already in use when they meet the requirement.
- Do not create alternate names for the same secret or token. Reuse the canonical name the user specified across code, Worker bindings, environment sync, and documentation.
