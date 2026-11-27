# Security Policy

This is the default security policy of Safe Labs GmbH for the repositories in this organization. A repository that has its own `SECURITY.md` follows that file instead.

## Where to Report

| What you found | Where it goes |
| --- | --- |
| A vulnerability in code in this organization, or in a service operated by Safe Labs (Safe{Wallet} web and mobile, backend services and APIs, SDKs, deployment registries, infrastructure code) | This policy. See [Reporting a Vulnerability](#reporting-a-vulnerability). |
| A vulnerability in the Safe Smart Account contracts or modules | The Safe Ecosystem Foundation, which maintains them in a separate organization and runs its own bug bounty program. See <https://docs.safe.global/advanced/smart-account-bug-bounty>. |
| A vulnerability in a third-party Safe App, a fork, or a project that integrates Safe | The maintainers of that project. |
| A phishing site or an account impersonating Safe | `security@safe.global`, with the address of the site or account. |
| A bug with no security impact | A public issue on the affected repository. |

## Reporting a Vulnerability

Please do not report security vulnerabilities through public GitHub issues, discussions, or pull requests.

Use GitHub's private vulnerability reporting on the affected repository:

1. Open the repository's **Security** tab.
2. Select **Advisories**.
3. Select **Report a vulnerability**.

If private vulnerability reporting is not available for the repository, or the issue affects a running service and not a specific repository, write to `security@safe.global`.

If user funds are at risk or a vulnerability is being exploited right now, write to `security@safe.global` and start the subject line with `URGENT`.

Please include as much of the following as you can:

- The affected repository, file, and version or commit, or the affected service and address.
- A description of the vulnerability and its potential impact.
- Steps to reproduce, or a proof of concept.
- Any required permissions, tools, or configuration.
- Suggested mitigations, if known.
- Whether the vulnerability is already public or being actively exploited.

Never include real private keys, seed phrases, access tokens, personal information, or other production secrets in a report.

## Scope

In scope:

- Code in the active, non-archived repositories of this organization.
- Packages and container images that Safe Labs publishes from these repositories.
- Production services operated by Safe Labs under `safe.global`.

We are most interested in issues that could lead to:

- Loss or freezing of user funds, or a transaction being executed that differs from what the user approved.
- Wrong or incomplete information shown to a user at the moment of signing.
- Tampering with transactions, signatures, or Safe configuration in our services or SDKs.
- Wrong contract addresses or ABIs in the deployment registries.
- Compromise of our build, release, or package publishing process.
- Unauthorized access to user data or to our infrastructure.

Out of scope:

- Smart contracts, third-party Safe Apps, forks, and integrations. See [Where to Report](#where-to-report).
- Archived repositories and releases that are no longer supported.
- Findings from automated scanners without a demonstrated security impact.
- Missing security headers, missing rate limits, or other best practice gaps without a demonstrated security impact.
- Vulnerabilities in third-party dependencies that are already public, unless you can show they are exploitable in our code.
- Attacks that require a compromised device, physical access, or a user ignoring a clear warning.
- Social engineering, phishing, or physical attacks against Safe Labs staff, contractors, or users.
- Denial of service through volume.

## Rules for Testing

- Test only against Safes, accounts, and data that you own, and prefer test networks.
- Do not access, change, or delete data that belongs to other people. If you come across personal data or secrets, stop, do not keep or share them, and tell us.
- Do not degrade or interrupt our services, and do not run high-volume automated scans against production.
- Use a finding only as far as needed to show that it exists.
- Do not disclose the issue to anyone else before it is resolved, except as described under [Disclosure](#disclosure).
- Follow the laws that apply to you.

## Safe Harbor

Safe Labs considers security research that follows this policy and is carried out in good faith to be authorized. We will not take legal action against you or file a criminal complaint for such research, and we will not treat it as a breach of our terms of use.

This statement covers only Safe Labs and the systems we operate. We cannot authorize testing of systems that belong to others, such as cloud providers, blockchain networks, or third-party applications, and we cannot speak for other parties or for public authorities. If someone else takes action against you for research that followed this policy, we will say that you acted in line with it.

If you are not sure whether something is allowed, ask us at `security@safe.global` before you go further.

## What to Expect

- We aim to acknowledge your report within 3 working days.
- We will keep you informed while we investigate and tell you when the issue is resolved.
- If the report belongs to another party, such as the Safe Ecosystem Foundation, we will tell you and, with your agreement, pass it on.

## Disclosure

We follow coordinated disclosure. Please give us up to 90 days from your report to fix the issue before you make it public. We may ask for more time when a fix needs coordination with other parties, and we will explain why.

Once a fix is released we publish a GitHub security advisory on the affected repository where that helps users. We credit reporters in the advisory unless they prefer to stay anonymous.

## Rewards

Safe Labs does not run a bug bounty program for the repositories and services covered by this policy. We may offer a reward for a report, entirely at our discretion. Submitting a report does not create a right to a reward, and nothing in this policy is a promise of one. Any reward is subject to applicable law, including sanctions rules.

## Supported Versions

Security fixes are provided for the latest release and the default branch of each repository. Older releases are not supported unless the repository says otherwise. For published packages, fixes are shipped as a new release and announced in a GitHub security advisory.

## Your Data

We use the personal data in your report only to handle the report and to contact you about it. See <https://safe.global/privacy>.
