# Privacy

This page explains what UdhaarLedger stores and when it uses the network. It
describes the app's behaviour, not a legal contract.

## Local-first

- The ledger is stored on your device.
- The local database is encrypted, and the app is unlocked with your PIN or an
  enabled device unlock method.
- The app does not include advertising, analytics, or crash-reporting SDKs.

## Backups

- Exported `.khb` backups are encrypted before they leave the app.
- Restoring a backup on a new device requires the recovery code that was active
  when the backup was made.
- Backup files are stored wherever you choose to save or share them. They are not
  deleted when you erase the app's local data.

## Optional cloud sync

Cloud sync is off unless you sign in and use it.

- The app uploads the encrypted portable snapshot, not plaintext ledger entries.
- The account profile stores the recovery salt and verifier needed to restore.
- If **Password-free restore** is enabled, the profile also stores a wrapped copy
  of the data key. Anyone who can sign in to that account can access the ledger
  while this is on.
- If password-free restore is off, the cloud account does not hold the key needed
  to decrypt the ledger.

## Update checks

The app checks a public version manifest once a day for a newer release. The check
does not require an account and does not send ledger data. Choosing **Download**
opens the download link in your browser.

## Notifications

Daily-save reminders are local notifications. No push-notification service is
used.

## Biometrics

Fingerprint and face unlock are handled by your device's operating system. The app
does not receive or store biometric data.

## Network use

The app uses the network only for:

- optional cloud sign-in and sync;
- update checks and downloads you start; and
- sharing an exported backup to another app or location, when you choose to.

## Removing data

- **Erase everything** in the app removes the local ledger and settings on that
  device.
- Encrypted cloud snapshots are separate. If you used cloud sync, remove the cloud
  data from that account when you no longer need it.
- Exported backup files must be deleted separately.

## Questions

Open an
[issue](https://github.com/david-ojah/udhaarledger-releases/issues) for general
privacy questions. Do not include real ledger data, PINs, recovery codes, or
account passwords. For security reports, use
[private vulnerability reporting](https://github.com/david-ojah/udhaarledger-releases/security/advisories/new).
