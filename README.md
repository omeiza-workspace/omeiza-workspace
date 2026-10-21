# Omeiza Okuta

**Open Source Architect** — building light, sustainable developer infrastructure
and local-first CI/CD automation.

I write the tools that decide whether a team waits forty seconds or forty
minutes for a green build, and I publish how every number was measured —
including the measurement I threw away and the claims I do not make.

**[Portfolio, case studies and public evidence →](https://omeiza-workspace.github.io/)**

---

## The tools

| | |
|---|---|
| **[CI Kit](https://github.com/omeiza-workspace/ci-kit)** — run your CI on your laptop, before you push. A local gate that runs the same scripts your GitHub Actions workflow runs, and runs the workflow itself locally through [`act`](https://github.com/nektos/act). Shell, MIT. | 99 s on a 2022 Intel laptop, against 43–48 s on a runner. It is a **guarantee of feedback, not a speedup** — and the [evidence document](https://github.com/omeiza-workspace/ci-kit/blob/main/docs/EVIDENCE.md) says so. |
| **[api-mock-services](https://github.com/omeiza-workspace/api-mock-services)** — stand-ins for the outside world. One dependency-free Node process standing in for 18 third-party providers: Stripe, Paystack, Interswitch, Flutterwave, Monnify, YouVerify, Smile ID, Twilio, Resend, Xero and the rest. MIT. | 50 MB in one process, against 250 MB across four containers. 0.0% idle CPU against 7.9%. First request in 1.4 s against 20 s and rising. The footprint is a **build gate**, so the number cannot quietly stop being true. |

## Why these two

Both exist because of a specific failure, not a feature list.

- On 21 October 2026, a repository had **28 failing runs out of the last 30** — and not one had failed on code. GitHub had refused to start the jobs over a spending limit, every run failing in about six seconds. Nobody could tell the difference between a red build and a build that never ran. CI Kit is the answer to that.
- The mock environment it grew alongside was **four containers, 250 MB, 7.9% idle CPU**, and a 214 MB OpenAPI proxy that never finished translating. api-mock-services is the answer to that.

## What I write about

Long-form technical essays on CI/CD reproducibility, offline-first integration
testing, and the discipline of publishing a measurement honestly.

- [The Silent Bill: How a Billing Decision Looked Like 28 Failed Builds](https://omeiza-workspace.github.io/blog/the-silent-bill-remote-ci-cd-drift/)
- [Architecting Local Sandboxes for Interswitch and Paystack Integrations, Completely Offline](https://omeiza-workspace.github.io/blog/architecting-local-sandboxes-offline/)
- [Deterministic Toolchains Don't Need a Backend](https://omeiza-workspace.github.io/blog/deterministic-toolchains-dont-need-a-backend/)
- [The Green Build Myth](https://omeiza-workspace.github.io/blog/the-green-build-myth/)
- [The earlier archive, 2013–2026](https://omeiza-workspace.github.io/archive/) — 30 articles, dated and unchanged.

## Where else

- **Portfolio and evidence** — https://omeiza-workspace.github.io/
- **[Open Source Impact](https://omeiza-workspace.github.io/evidence/)** — the consolidated public record
- **[Endorsement evidence map](https://omeiza-workspace.github.io/endorsement/)** — every claim, and the artefact that supports it
- **[LinkedIn](https://www.linkedin.com/in/omeiza-okuta)** · **[X](https://x.com/omeiza)** · **[RSS](https://omeiza-workspace.github.io/feed.xml)**

## Elsewhere in the workspace

| | |
|---|---|
| **[homebrew-tap](https://github.com/omeiza-workspace/homebrew-tap)** | Homebrew formulas for the tools in this workspace |
| **[TechLiaison](https://github.com/omeiza-workspace/TechLiaison)** | The original Hugo blog, before it moved to the portfolio |
| **[omeiza-workspace.github.io](https://github.com/omeiza-workspace/omeiza-workspace.github.io)** | This site's source — JSON in, static HTML out, no dependencies |

---

<sub>Available for Global Talent visa endorsement enquiries. Technical and
endorsement questions: [okuta.omeiza@gmail.com](mailto:okuta.omeiza@gmail.com)</sub>
