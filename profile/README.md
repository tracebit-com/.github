# Tracebit

**Detect attacks in your environment at scale.**

Tracebit detects attackers in your environment in real time, with high fidelity, and at
scale. It is deception technology built for modern environments: canaries deployed as
infrastructure as code, kept fresh automatically by AI, so coverage scales to your entire
estate without going stale or ballooning operational cost.

Tracebit deploys canaries wherever an attacker actually lands, across cloud accounts,
identity, SaaS, CI/CD, workstations and perimeter sensors, as code, in a single motion.

## What is a canary?

A canary is a decoy credential or resource with no legitimate production use. A trigger gives you a high-confidence signal to investigate. Credential canaries alert when someone attempts to use them.

## Open source

**[tracebit-community-cli](https://github.com/tracebit-com/tracebit-community-cli)**
Command-line tool for Tracebit Community Edition. Deploys and maintains canary AWS
credentials, SSH keys, browser cookies, website passwords and emails across
your devices and accounts. MIT licensed.

**[tracebit-community-action](https://github.com/tracebit-com/tracebit-community-action)**
GitHub Action that injects canary AWS credentials and SSH keys into your build pipelines,
so use of credentials harvested by a compromised dependency or action triggers an alert. MIT licensed.

**[awesome-deception](https://github.com/tracebit-com/awesome-deception)**
Curated list of articles, research, guides, talks and tools on cybersecurity deception.
Contributions welcome.

**[tracebit-canary-honeytokens-skill](https://github.com/tracebit-com/tracebit-canary-honeytokens-skill)**
Agent skill for end-to-end canary coverage using Tracebit Community Edition.

## Research

**[Context Bombs](https://agentic.tracebit.com/context-bombs/)** — our research into
disrupting AI attackers as well as detecting them. A context bomb is text placed inside a
canary to trigger an attacking model's safety guardrails. Our working paper reports tests
across five frontier models and 152 attack runs. Results depend on the model and attack;
see the research for methods, outcomes and limitations.

The trigger strings are published at
[context-bombs](https://github.com/tracebit-com/context-bombs).

Other work:

- [Prompt injection against Gemini CLI, a worked example](https://github.com/tracebit-com/gemini-cli-injection-example)
- [Finding the AWS Account ID behind an S3 bucket](https://github.com/tracebit-com/find-s3-account)
- [Investigating CloudTrail latency with Athena](https://github.com/tracebit-com/cloudtrail-latency-investigation)

More at [tracebit.com/blog](https://tracebit.com/blog).

## Getting started

Community Edition is free. Create an account at
[community.tracebit.com](https://community.tracebit.com) and [install the CLI](https://github.com/tracebit-com/tracebit-community-cli#getting-started), then connect
it with `tracebit auth` and place your first canaries with `tracebit deploy all`.

For cloud accounts, identity providers, CI/CD and Kubernetes at scale, see
[tracebit.com](https://tracebit.com). Common questions about canaries and deception
technology are answered at [ai.tracebit.com](https://ai.tracebit.com).
