# Version history

Download builds from the
[Releases page](https://github.com/david-ojah/udhaarledger-releases/releases).

## 1.1.1 — 2026-11-20

- Android builds now use the permanent release signing key.
- Devices with the earlier debug-signed build must uninstall it once before
  installing 1.1.1. Restore your data from an encrypted backup or your cloud
  account afterwards.

## 1.1.0 — 2026-11-20

- Added manual **Save to cloud** (upload only) and **Sync now** (download, merge,
  then upload).
- Added **Unsynced changes** tracking.
- Added opt-in daily save at a chosen time, defaulting to 22:00, with a local
  reminder when the app is closed.
- Added optional password-free restore using a cloud account.
- Added cloud-account PIN reset for a forgotten PIN.
- Improved biometric unlock, including device-credential fallback.
- Added in-app update checks with dismissible update prompts.
- Fixed cloud bookkeeping so saving no longer marks the ledger as changed again.

## 1.0.0

The initial release is superseded by 1.1.0 and is no longer distributed.

- Initial release.
- Offline customer ledger with credit and payment entries, balances, and reports.
- English and Assamese interfaces.
- Four-digit PIN, biometric unlock, and recovery code.
- Encrypted portable backups.
