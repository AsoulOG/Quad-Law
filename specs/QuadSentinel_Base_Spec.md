# QuadSentinel Specification

## Purpose
QuadSentinel defines a deterministic standard for verifying whether an artifact
conforms to OriginSTANDARD authenticity requirements.

This specification describes observable verification behavior only.
It does not describe how authenticity is generated.

## Standard Output
A Standard Output is any artifact that:
- Contains an embedded OriginSTANDARD authenticity marker (“Glow”)
- Is accompanied by a signed receipt (“Seal”)
- Passes verification under this specification

## Verifier Behavior
A conforming verifier MUST:
- Accept an artifact and its receipt
- Perform deterministic validation checks
- Output exactly one result: PASS, FAIL, or INVALID

A verifier MUST NOT:
- Modify data
- Infer intent or meaning
- Score, rank, or estimate confidence
- Issue or sign artifacts

## Authority Boundary
Verification is public and permissionless.
Issuance and signing authority are reserved.

Possession of this specification does not grant issuance rights.

## Non-Goals
This specification does not attempt to:
- Prove truth, ownership, or legality
- Judge content or value
- Replace human responsibility.
