# Jargon Buster

Plain-English explanations of the technical words in this project. The README does not use these words when it can. This file gives the exact words for readers who want them.

**A2A (Agent-to-Agent)**
A protocol that lets one AI agent find another agent and give it tasks. ANAB has extra rules for agents that use A2A.

**Agent Card**
A machine-readable file that describes an A2A agent: its name, its operator, its endpoints, and its sign-in rules. It must agree with the Agent Page.

**Agent Name**
The friendly name of an AI agent, for example "travel-helper". ANAB treats the name only as a hint. The name alone does not prove anything.

**Agent Page**
The public web page of an agent. It shows who operates the agent and where to find the proof.

**Applicability matrix**
A table in the source project. It shows which controls apply to each profile. Each control is a "must", a "should", a "conditional", or "not required".

**Assurance Level (AL1 to AL4)**
A measure of how good your evidence is. AL1 means that the evidence is complete. AL4 means continuous checks and regular audits. AL2 and higher need an evidence bundle.

**Binding**
The connection between the agent name and a cryptographic key. A strong binding is signed and a visitor can check it.

**Conformance declaration**
A signed file that states your tier, your profile, your assurance level, and the controls that you use. It has a link to the evidence for each control.

**Control**
One rule in the baseline. Each control has an ID, for example `ANAGB-UI-01`.

**Cryptographic ID**
A unique identifier that a cryptographic key controls. In ANAB, this is usually a DID.

**DID (Decentralized Identifier)**
A type of cryptographic ID that no single company controls. A DID points to a DID document that holds the public keys and the endpoints.

**Drift**
An unexpected change in the binding or the endpoints, for example after an attacker takes control of a domain. ANAB requires that you monitor for drift.

**Endpoint**
The web address where a program or an agent receives requests.

**Evidence bundle**
A package of files that proves your claims: logs, settings, test results, and runbooks. It has a `bundle.json` file that lists the files.

**Fail safe**
When the proof is missing, old, or not clear, the visitor does not increase trust. The visitor does not assume the best case.

**Profile**
What your agent is permitted to do. The four profiles are Core, Deploy, Transact, and Enterprise. Each profile has a minimum tier.

**Relying party (visitor)**
A person or an agent that uses your agent and relies on its name. The diagrams call this the "visitor".

**Revocation**
The cancellation of a key or a credential, for example after a compromise. Higher tiers need faster revocation checks.

**Schema**
A file that tells a program the correct shape of a data file. A schema check finds missing or incorrect fields.

**Step-up verification**
An extra check before a high-risk action, for example a payment. The extra check can be a human approval or a stronger sign-in.

**Tier (AN-0 to AN-3)**
The strength of the proof that connects the name to the key. AN-0 is weak. AN-3 is very strong.

**TLS**
The encryption that protects a web connection. Web addresses that start with `https` use TLS.

**Transparency log**
A public record that anyone can read. Each change to the binding goes into the log, so that nobody can make a secret change.

**Verifiable Credential (VC)**
A signed digital statement from an issuer, for example "this organization owns this agent". A visitor can check the signature.
