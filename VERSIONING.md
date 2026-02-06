# Versioning and Stability Policy (AMPL)

This document describes the versioning policy for the Acipe Minimal Permissive
License (AMPL) and the stability guarantees associated with AMPL-1.0.

AMPL is intended to be stable, minimal, and long-lived.

---

## 1. AMPL-1.0 Is Frozen

The text of the Acipe Minimal Permissive License v1.0 (AMPL-1.0) is considered
final and permanent.

**First published:** 2026-02-05

- The canonical AMPL-1.0 license text is located in `LICENSE.txt`.
- AMPL-1.0 will not be modified, amended, or reinterpreted through later edits.
- Typographical corrections to the repository copy may be made only if they
  restore the canonical intended text and do not alter meaning.

This stability guarantee exists so that developers and organizations may adopt
AMPL-1.0 without concern that the license terms will drift over time.

---

## 2. Future Versions Are Opt-In Only

If future versions of AMPL are published (e.g., AMPL-1.1, AMPL-2.0):

- they will be released under a new version number,
- they will be published as separate, distinct license texts,
- they will not apply retroactively to software licensed under AMPL-1.0,
- projects may continue using AMPL-1.0 indefinitely.

No project is expected or required to upgrade.

---

## 3. Semantic Versioning Guidance

AMPL version numbers are intended to be meaningful.

- **Patch changes** (e.g., 1.0.1) are not used for license text changes.
  License text does not receive patch updates.

- **Minor version changes** (e.g., 1.1) may be used only for clarifications or
  additions that do not reduce permissions but are still significant enough to
  justify a new license text.

- **Major version changes** (e.g., 2.0) may be used for substantial revisions,
  restructuring, or changes in scope.

AMPL does not promise that future versions will be compatible with earlier ones.
Only AMPL-1.0 is guaranteed to remain unchanged.

---

## 4. Documentation Is Not the License

Supporting documentation may evolve over time, including:

- FAQs
- examples
- comparison tables
- historical background
- reviewer notes

These materials are provided for education and clarity only.

They do not modify, override, or replace the binding legal terms of AMPL-1.0.
Only the text of `LICENSE.txt` defines AMPL-1.0.

---

## 5. SPDX Identifier Guidance

Until AMPL is accepted into the SPDX License List, projects should use:

    SPDX-License-Identifier: LicenseRef-AMPL-1.0

If AMPL is later accepted into SPDX under an official identifier, projects may
choose to update their source headers to use the official identifier, but doing
so is optional.

---

## 6. Summary

- AMPL-1.0 is frozen and permanent.
- AMPL-1.0 was first published on 2026-02-05.
- Future versions, if any, will be opt-in and separately versioned.
- Documentation may change, but the license text will not.
- SPDX should use `LicenseRef-AMPL-1.0` until an official identifier exists.
