# ci-cd-continuity-guard: Automated Verification & Assertions (`SUBVERTED_HARRY`)

[![Repo Type: Automated CI/CD](https://img.shields.io/badge/Repo-Continuity%20Guard-red.svg)](https://github.com/ImmortalWiz/ci-cd-continuity-guard)
[![Enforcement: Automated Verification](https://img.shields.io/badge/CI-Automated%20Assertions-brightgreen.svg)](https://github.com/ImmortalWiz/ci-cd-continuity-guard)
[![Parent Engine](https://img.shields.io/badge/Parent-harry--potter--and--the--magical--reality--check-blue.svg)](https://github.com/ImmortalWiz/harry-potter-and-the-magical-reality-check)

The **Continuity Guard (`ci-cd-continuity-guard`)** repository contains the automated verification rules, assertion specifications, and dependency compiler for the entire `SUBVERTED_HARRY` engine. It ensures that complex worldbuilding, character trauma, and spell mechanics remain logically bulletproof across multiple volumes.

---

## 🛡️ Core Assertion Suites

```
ci-cd-continuity-guard/
├── compile_dependency_checks.md        # Protocols for tracing cross-repository dependencies
└── validation_assertions/
    ├── blood_protection_assert.md     # Asserts Petunia's household maintains protection conditions
    ├── magic_gap_assert.md            # Checks Harry has not cast a spell above his active ledger
    └── psychological_inertia_assert.md # Asserts Harry's personality shifts are gradual and earned
```

---

## 🔍 Assertion Specifications

### 1. The Magic Gap Assertion (`magic_gap_assert`)
* **Trigger:** Runs against all new commits in `scene-blueprints/` and `prose-drafts/`.
* **Logic:** Cross-references any spell named in prose or blueprint against `characters/harry_potter/magical_gap_ledger.md`.
* **Failure Condition:** If Harry successfully casts an untested foundational spell or performs theoretical deduction without prior study, the check **FAILS**.

### 2. Blood Protection Assertion (`blood_protection_assert`)
* **Trigger:** Runs against `wbc-library/` theological/ward files and Privet Drive scenes.
* **Logic:** Validates that Lily's sacrificial ward remains tied to blood-kinship and residence requirements.
* **Failure Condition:** If Harry abandons Number Four Privet Drive without triggering the collapse of the blood wards or foreign faction tracking, the check **FAILS**.

### 3. Psychological Inertia Assertion (`psychological_inertia_assert`)
* **Trigger:** Runs against character state mutations in `war-entities/`.
* **Logic:** Enforces that coping mechanisms (Lockhart bravado, paranoia, hyper-vigilance) diminish only through gradual, traumatic deconstruction rather than sudden epiphanies.
* **Failure Condition:** Any sudden "healing" or unearned emotional maturity without narrative cause **FAILS**.

---

## 🤖 Instructions for AI Context Verification

When validating a generated scene or chapter, execute this exact evaluation prompt:

```text
[CONTINUITY VERIFICATION PROTOCOL]
Review the prose draft generated against the following assertions:
1. Cross-reference all magic with Harry's active magical_gap_ledger.md.
   Identify any spell requiring fundamentals Harry has not mastered.
2. Verify that supporting characters (Snape, Dumbledore, Hermione) act from
   their documented behavioral blindspots rather than magically discovering Harry's abuse.
3. Verify that sensory descriptions align with WBC cosmological and environmental laws.
OUTPUT FORMAT: Output 'CONTINUITY CHECK: PASS' or list specific failure points with file references.
```

---

## 👤 Guide for Contributors

* **Adding New Assertions:** When introducing new magical phenomena or complex political factions in `wbc-library`, add a corresponding assertion file in `validation_assertions/` defining the logical boundaries.
* **CI Integration:** Automated GitHub Actions workflows invoke these assertion rules against pull requests touching `scene-blueprints` and `prose-drafts`.
