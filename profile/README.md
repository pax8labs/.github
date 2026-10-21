# Pax8 Labs

Pax8 Labs is the R&D and product innovation team at [Pax8](https://www.pax8.com). We run
experiments, test ideas with MSPs, and ship early so we can learn quickly. Projects that prove
themselves graduate into Pax8's broader product portfolio.

Here we publish open-source tools for MSPs and the people who build for them. They work the same
way for a person at a terminal, a shell script, or an AI agent.

> **Expect things to move.** Labs projects evolve quickly. We want your feedback, and an issue
> telling us what's missing or broken is one of the most useful things you can send.

## Projects

| Project | What it does | Install |
|---|---|---|
| [**pax8-cli**](https://github.com/pax8labs/pax8-cli) | Command-line tool for Pax8 marketplace operations: subscriptions, billing, renewals, invoice audit, and upsell recommendations. Every command supports `--json`. | `npx -y -p @pax8/cli pax8 --help` |
| [**pax8-cta**](https://github.com/pax8labs/pax8-cta) | Cross-Tenant Agents: deploy Microsoft Copilot Studio agents to many customer tenants via GDAP, with staged rollouts and rollback. | `npx -y -p @pax8/cta pax8-cta --help` |
| [**homebrew-tap**](https://github.com/pax8labs/homebrew-tap) | Homebrew formula for the Pax8 CLI. | `brew install pax8labs/tap/pax8` |

Both CLIs have a **demo mode** with sample data, so you can try them without credentials:

```bash
PAX8_DEMO=1 npx -y -p @pax8/cli pax8 dashboard
DEMO_MODE=true npx -y -p @pax8/cta pax8-cta tenants list
```

## Contributing

We welcome issues and pull requests. Each repository has its own README covering setup and
contribution details. If something doesn't work, please open an issue on that project.
Please don't include real customer data, tenant IDs, or credentials in issues or logs.

## Contact

Questions, partnership ideas, or feedback that doesn't fit an issue? Email us at
[labs@pax8.com](mailto:labs@pax8.com).

## Security

If you find a security vulnerability, please **do not** open a public issue. Report it privately
through GitHub's [private vulnerability reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability)
on [pax8-cli](https://github.com/pax8labs/pax8-cli/security) or
[pax8-cta](https://github.com/pax8labs/pax8-cta/security) (see each repo's `SECURITY.md`).
The Homebrew formula is generated from pax8-cli, so report tap issues there. For anything else,
email [labs@pax8.com](mailto:labs@pax8.com).

## License

pax8-cli and pax8-cta are released under the [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license.
