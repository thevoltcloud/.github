# Security Policy

> Based on the [OpenSSF OSS Vulnerability Guide](https://github.com/ossf/oss-vulnerability-guide) GitHub security policy template, localized for Volt.

## Reporting a Vulnerability

To report a security issue, please email **security@voltcloud.ai** with a description of the issue, the steps you took to create the issue, affected versions, and, if known, mitigations for the issue. Our vulnerability management team will respond within 3 working days of your email. If the issue is confirmed as a vulnerability, we will open a GitHub Security Advisory. This project follows a 90 day disclosure timeline.

Please **do not** open a public GitHub issue for security reports.

## Encrypted reporting

`security@voltcloud.ai` accepts GPG-encrypted mail. The current public key and its fingerprint are published at:

```
https://voltcloud.ai/.well-known/security.txt
```

(per [RFC 9116](https://www.rfc-editor.org/rfc/rfc9116)). Use it for any report containing sensitive details, proof-of-concept code, or customer data.

## Scope

This policy is the org-wide default for every repository under [`thevoltcloud`](https://github.com/thevoltcloud). A repository that ships its own `SECURITY.md` overrides this one. It covers Volt's first-party code (SDKs, `voltctl`, services, platform). For vulnerabilities in upstream CNCF projects we fork (llm-d, KServe, Kueue, Cilium, SPIRE, vLLM), please also follow that project's disclosure process.

## What to expect

- Acknowledgement within **3 working days**.
- A coordinated fix and GitHub Security Advisory if confirmed.
- A **90-day** coordinated disclosure timeline, adjustable by mutual agreement for complex issues.
- Credit in the advisory unless you ask to remain anonymous.

Thank you for helping keep Volt and its users safe.
