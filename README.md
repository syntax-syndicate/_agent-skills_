# Skills

Personal coding-agent skills for TypeScript engineering, architecture, Cloudflare composition, and agent workflows.

## Included skills

- `coding-standards/` — model-invoked, correct-by-construction TypeScript standards covering typed failures, boundary parsing, domain modeling, modules and adapters, workflows, testing, and TypeScript safety.
- `bootstrap-prelude/` — model-invoked workflow for bootstrapping a TypeScript `prelude.ts` from the bundled foundation and ambient generic helpers and types discovered across the target repository.
- `cloudflare-composition-root/` — model-invoked guidance for keeping Cloudflare bindings and runtime types at Hono and Worker composition roots. Includes concrete Hono, `WorkerEntrypoint`, adapter, and refactor examples in `EXAMPLES.md`.
- `tech-spec/` — user-invoked, design-only workflow for producing typed call-stack architecture handoffs with alternatives, contracts, seams, data flows, file changes, and an RGR TDD plan.
- `herdr/` — model-invoked instructions for managing herdr workspaces, tabs, panes, sibling agents, servers, output, and wait conditions. Applies only inside a herdr-managed pane (`HERDR_ENV=1`).
- `bro/` — user-invoked request to restate the previous response plainly and concisely.

Each skill uses `SKILL.md` as its entrypoint. Supporting templates and examples are colocated with the skill that owns them.

### Vendored from Matt Pocock

These skills are vendored from [mattpocock/skills](https://github.com/mattpocock/skills) so the collection is self-contained. Do not edit them by hand; re-sync instead.

- `grilling/` — model-invoked relentless interview loop.
- `grill-me/` — user-invoked grilling session.
- `domain-modeling/` — model-invoked glossary and architectural-decision workflow.
- `grill-with-docs/` — user-invoked grilling session that also builds docs such as ADRs and a glossary.
- `tdd/` — model-invoked red-green-refactor test-driven development.

Resync with:

```sh
scripts/sync-matt-skills.sh                 # from upstream main
MATT_SKILLS_REF=<sha|tag|branch> scripts/sync-matt-skills.sh
```

## Design principles

- Prefer correct-by-construction APIs, explicit dependencies, typed failures, and parsed boundary values.
- Keep domain and application code independent of frameworks, protocols, vendors, and runtime bindings.
- Prefer deep, cohesive modules and real test seams over pass-through abstractions, module mocks, and spies.
- Use code-shaped contracts, call stacks, and concrete evidence when design precision matters.
- Keep deliberate workflows user-invoked.

## Credits

Thanks to Matt Pocock for inspiration around writing high-quality agent skills, especially the `writing-great-skills` skill and its emphasis on predictable execution, progressive disclosure, context pointers, completion criteria, and pruning duplication.
