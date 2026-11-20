# Cloud sync

Cloud sync is optional. Without it, UdhaarLedger works entirely offline and keeps
everything on your device.

## Signing in

- **Android:** sign in with a Google account.
- **Windows:** sign in with an email address and password. Google sign-in is not
  available on Windows.

Your local ledger is never replaced just by signing in. Signing out leaves the
local data and any unsynced changes on the device.

## Manual save and sync

- **Save to cloud** uploads local changes only.
- **Sync now** downloads newer cloud changes, merges them, then uploads local
  changes.
- The **Unsynced changes** label means local edits have not been uploaded yet.

The app does not upload after every entry. Use **Save to cloud**, **Sync now**, or
the daily save option to control when cloud usage happens.

## Daily save

Daily save is off by default. When enabled:

- The app saves once a day at the time you choose. The default is 22:00.
- If the app is open at that time, it saves then.
- If the app was closed, a local notification reminds you, and the save runs on
  the next unlock.
- If you are offline or signed out, the save is skipped and retried on the next
  open.

## Password-free restore

This is off by default. When enabled, a wrapped copy of your key is kept in your
cloud account so that:

- a new device can restore after signing in without the recovery code; and
- a forgotten PIN can be reset from the signed-in account.

**Trade-off:** anyone who can sign in to your account can access your ledger while
this is on. Your recovery code remains the higher-security option because it is
not stored in the account.

You can turn password-free restore off in **Settings → Cloud sync**. Doing so
removes the wrapped key from the account.

## Restoring on a new device

1. Install UdhaarLedger and choose the restore option on the lock screen.
2. Sign in to the same cloud account.
3. If password-free restore is enabled, choose **Restore with my account**.
4. Otherwise, enter your recovery code.

After restoring, run **Save to cloud** once if you want the restored ledger to
become the cloud copy.

## What is uploaded

Only the same encrypted portable snapshot used by `.khb` backups, plus account
profile data needed for restore. The ledger contents are encrypted before upload.

See [Privacy](PRIVACY.md) for the full picture.
