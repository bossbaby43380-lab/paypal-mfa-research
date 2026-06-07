# PayPal Research Log

> Ongoing security research and authentication analysis conducted against in-scope PayPal assets under the HackerOne Bug Bounty Program.

---

# Overview

This repository documents ongoing research focused on:

* MFA / 2FA enforcement
* Step-Up authentication
* SCA (Strong Customer Authentication)
* Authentication state transitions
* Cross-channel authentication behavior
* Edge infrastructure observations
* Differential API behavior analysis

The purpose of this repository is to maintain:

* structured documentation,
* reproducible observations,
* MITRE ATT&CK-aligned methodology,
* and a continuously updated research timeline.

---

# Scope Alignment

Research is being conducted in accordance with:

* PayPal HackerOne Bug Bounty Program
* PayPal MFA Bypass Campaign
* HackerOne Platform Standards

Current testing is limited to:

* passive reconnaissance,
* authentication workflow analysis,
* request/response observation,
* low-impact differential testing.

No destructive testing, brute forcing, denial-of-service activity, credential stuffing, or unsafe automation is being performed.

---

# Research Methodology

## Frameworks

This research follows methodologies inspired by:

* MITRE ATT&CK
* Authentication state machine analysis
* Adversarial workflow modeling
* Differential edge behavior analysis

---

# MITRE ATT&CK Mapping

## TA0043 — Reconnaissance

### Techniques

* Active Scanning
* Gather Victim Network Information
* Gather Victim Host Information

### Objectives

* Identify exposed edge infrastructure
* Map alternate HTTPS surfaces
* Observe authentication-related routing behavior

---

# Infrastructure Reconnaissance

## Identified Infrastructure IP

173.0.92.23

Observed behavior suggests association with infrastructure serving PayPal-related HTTPS traffic.

---

# Open Ports Observed

| Port | Service |
| ---- | ------- |
| 80   | HTTP    |
| 443  | HTTPS   |
| 2052 | HTTP    |
| 2053 | HTTPS   |
| 2082 | HTTP    |
| 2083 | HTTPS   |
| 2086 | HTTP    |
| 2087 | HTTPS   |
| 2095 | HTTP    |
| 2096 | HTTPS   |
| 8080 | HTTP    |
| 8443 | HTTPS   |

---

# TLS Observations

The following observations were made during TLS enumeration:

* Certificates referenced `api.paypal.com`
* Alternate HTTPS ports reused similar certificate chains
* Cloudflare-related behavior was consistently observed
* ALPN negotiation supported HTTP/2

---

# HTTP Behavior

## Raw IP Access

Direct browser access to the identified IP returned:

```http
HTTP/1.1 403 Forbidden
Server: cloudflare
```

This behavior suggests:

* hostname-based routing,
* reverse proxy enforcement,
* or expected Cloudflare edge filtering.

No unauthorized access or security bypass condition has been identified at this stage.

---

# Initial Research Hypotheses

The following hypotheses are currently under investigation:

1. Authentication behavior may differ across alternate HTTPS ports.
2. MFA enforcement logic may vary between:

   * web flows,
   * mobile APIs,
   * alternate edge listeners,
   * and cross-channel authentication states.
3. Step-Up enforcement may rely on trust assumptions between services.
4. Session state synchronization inconsistencies may exist.

These remain hypotheses only and have NOT been validated.

---

# Authentication Research Objectives

Current priorities include:

* Mapping login state transitions
* Capturing MFA challenge workflows
* Identifying authentication state tokens
* Comparing behavior across:

  * web flows,
  * mobile flows,
  * alternate HTTPS surfaces
* Observing trusted-device behavior
* Investigating potential MFA downgrade paths

---

# Current Research Status

## Completed

* Initial infrastructure reconnaissance
* Port and TLS enumeration
* Cloudflare edge observation
* MITRE ATT&CK mapping
* Authentication surface identification

## In Progress

* Web authentication flow mapping
* MFA challenge-state analysis
* Session issuance analysis
* Cross-channel testing preparation

## Pending

* MFA replay testing
* State-transition testing
* Trusted-device analysis
* Differential edge authentication analysis
* Step-Up enforcement testing

---

# Research Principles

The following operational principles are being followed throughout this engagement:

1. Document everything.
2. Stay strictly within published scope.
3. Avoid service disruption.
4. Avoid unsafe automation.
5. Validate findings before disclosure.
6. Maintain reproducible evidence.
7. Prioritize authentication-impact analysis.

---

# Repository Structure

```text
/paypal-mfa-research
│
├── README.md
├── reconnaissance/
├── screenshots/
├── mitre-mapping/
├── notes/
└── reports/
```

---

# Planned Research Phases

## Phase 1 — Reconnaissance

* Infrastructure mapping
* Edge behavior analysis
* TLS and routing observation

## Phase 2 — Authentication Mapping

* Login workflow analysis
* MFA challenge-state capture
* Session issuance tracking

## Phase 3 — Differential Testing

* Alternate edge comparison
* Mobile/web comparison
* Cross-channel authentication analysis

## Phase 4 — Validation

* Reproducibility testing
* Impact confirmation
* Responsible disclosure preparation

---

# Disclaimer

This repository does NOT claim the existence of a confirmed vulnerability.

All findings documented here represent ongoing security research and infrastructure observations conducted within the context of authorized bug bounty testing.

Any confirmed vulnerabilities discovered during this research will be responsibly disclosed to PayPal through HackerOne prior to any public disclosure.
