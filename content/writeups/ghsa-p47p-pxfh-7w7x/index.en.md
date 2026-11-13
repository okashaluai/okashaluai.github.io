---
title: "Command injection in a biometric research tool: from bug to GHSA"
date: 2026-11-13
draft: true   # set to false when the post is finished
tags: [web, disclosure, cwe-78]
tldr: "TODO: one paragraph — what the bug is, where it lives, what an attacker gets, and that it is fixed."
summary_de: "TODO: 2–3 Sätze auf Deutsch – Schwachstelle, Auswirkung, Status."
advisory:
  id: GHSA-p47p-pxfh-7w7x
  url: https://github.com/okashaluai/Fingerprint-Biometric-Research-Tool/security/advisories/GHSA-p47p-pxfh-7w7x
  cve: requested
  cwe: 78
  cvss: ""
timeline:
  - date: "YYYY-MM-DD"
    event: Vulnerability found
  - date: "YYYY-MM-DD"
    event: Fix released
  - date: "YYYY-MM-DD"
    event: GHSA-p47p-pxfh-7w7x published
  - date: "YYYY-MM-DD"
    event: CVE requested
---

## Background

TODO: what the tool does and where untrusted input enters.

## Root cause

TODO: walk through the vulnerable code path.

```python
# TODO: vulnerable snippet
```

{{< callout >}}TODO: preconditions for exploitation, or a key insight.{{< /callout >}}

## Proof of concept

TODO

## Impact

TODO

## Fix

TODO: what changed, with the patch diff.
