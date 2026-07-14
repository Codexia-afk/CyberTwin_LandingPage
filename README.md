# CyberTwin AI

> **The Explainable AI Digital Trust Layer for the Browser**

CyberTwin AI is a privacy-first browser extension that helps users understand **what and whom they can trust online** before clicking a link, downloading a file, entering credentials, making a payment, opening an attachment, accepting a recruiter request, or continuing a suspicious digital interaction.

Unlike traditional phishing detectors that return only **Safe** or **Dangerous**, CyberTwin correlates identity, organization, behavior, historical context, links, attachments, social-engineering signals, and platform warnings to generate an explainable **Trust Score** with evidence, confidence, prediction, and actionable guidance.

---

## Problem Statement

Generative AI has fundamentally changed digital deception.

Fraudulent emails, fake recruiters, cloned websites, malicious QR codes, deepfake communication, fake OAuth requests, payment scams, and social-engineering attacks are becoming increasingly difficult to distinguish from legitimate interactions.

Most existing security tools evaluate threats in isolation and provide fragmented warnings without explaining:

- why an interaction is risky,
- how the decision was made,
- whether the behavior differs from past interactions,
- what may happen next,
- or what the user should do.

As a result, users face alert fatigue, uncertainty, and preventable security incidents.

CyberTwin AI addresses this by creating an **Explainable AI Digital Trust Layer** for the browser.

---

## Core Idea

Traditional tools ask:

> **“Is this phishing?”**

CyberTwin asks:

> **“Should you trust this interaction, why, what could happen next, and what should you do?”**

---

## Key Features

### Explainable Trust Score

CyberTwin generates a transparent Trust Score using evidence from:

- Identity trust
- Organization trust
- Authentication availability
- Link and destination analysis
- Social-engineering patterns
- Historical interactions
- Behavioral anomalies
- Platform-native warnings
- Context intelligence
- Threat indicators

Each score includes:

- Overall Trust Score
- Risk Score
- AI Confidence
- Evidence Quality
- Positive evidence
- Negative evidence
- Missing evidence
- Recommended action

---

### Universal Browser Trust Layer

CyberTwin is designed around a platform-adapter architecture rather than a Gmail-only scanner.

Supported interaction sources include:

- Gmail
- LinkedIn
- Outlook Web
- GitHub
- Generic websites

Every platform is normalized into a shared `TrustInteraction` model and processed by the same trust engine.

---

### Proactive Context Intelligence

CyberTwin does not wait only for manual scans.

It can detect unusual behavior such as:

- First-time payment requests
- First-time credential requests
- New destination domains
- Unexpected attachments
- New OAuth permissions
- Communication-style changes
- Organization-domain mismatches
- Unusual timing
- Cross-platform behavior changes

Example:

```text
Unusual request detected

This sender has contacted you 18 times,
but has never requested payment before.

The message also introduces a new domain
and uses urgency language.

Recommendation:
Verify through a separate communication channel.
