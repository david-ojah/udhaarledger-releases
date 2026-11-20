# Recovery and PIN help

## Your recovery code

The recovery code is shown when you first set up the app. It is the key to
restoring your ledger after a forgotten PIN or on a new device.

- Store it in a password manager or on paper, away from the phone or computer.
- Do not share it. Anyone with the code and a copy of your backup can read the
  ledger.
- It is shown only once. If you lose it and password-free restore is off, a
  forgotten PIN cannot be recovered.

## Forgot your PIN

The app offers these paths, depending on what is set up:

1. **Recovery code** — enter the code to regain access without erasing data.
2. **Fingerprint or face unlock** — if biometric unlock is enabled and the device
   still recognises you.
3. **Cloud account reset** — if password-free restore is enabled, sign in to the
   same account and reset the PIN. Your data is preserved.
4. **Erase everything** — permanently removes local data. Use this only when the
   other options are unavailable and the data is not needed.

## Moving to a new device

### With a cloud account

1. Install the app and choose the restore option.
2. Sign in to the same account.
3. Use **Restore with my account** when password-free restore is enabled, or enter
   the recovery code.

### With a backup file

1. Export an encrypted `.khb` backup from the old device
   (**Settings → Backup and restore → Export backup**).
2. Move the file to the new device.
3. On the new device, choose **Import backup** and enter the recovery code that
   was active when the backup was made.

## Changing the recovery code

Regenerating the recovery code creates new local snapshots. Older exported
backups will no longer restore, so export a fresh backup afterwards.

## If you cannot recover

There is no backdoor and no support override. Without the recovery code, the
cloud account option, or a usable biometric unlock, the encrypted data cannot be
opened. Keep the recovery code safe and export backups regularly.
