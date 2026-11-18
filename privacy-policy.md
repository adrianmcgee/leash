# Leash — Privacy Policy

_Last updated: November 18, 2026_

Leash ("the app") connects your iPhone, Apple Watch, and Mac so you can see and
respond to your AI coding agent (Claude Code and compatible CLIs) remotely. This
policy explains what data Leash handles and how.

**Summary: Leash encrypts the content that passes between your phone and Mac.
We use routing identifiers to deliver notifications and retain account identifiers
if you enable Account & Key Sync. Leash does not use analytics or sell data.**

## What Leash handles

- **Notification & session content** (the commands, prompts, plans, questions,
  and replies shown in the app). This is generated on your Mac and displayed on
  your devices.
  - **On the same Wi-Fi:** it travels directly between your devices over your
    local network. It never leaves your network.
  - **Off Wi-Fi:** it travels through an optional relay server as
    **AES-GCM-encrypted ciphertext**. The encryption key is derived from a
    pairing secret that only your devices hold. The relay sees an opaque room
    identifier and ciphertext — **it cannot read your content**.
    Encrypted notification envelopes may be retained for up to **7 days** so a
    phone that was offline can import missed events. They are deleted earlier after
    the phone confirms local storage.
- **Pairing secrets** are stored in the Apple **Keychain** on your devices.
  Account & Key Sync can store a copy encrypted for one of your devices. The
  relay cannot read the pairing secret.
- **Settings, paired-Mac records, and recent-notification history** are stored
  **locally** on your device (and shared with the Leash widget via an app group).
- **Apple Push Notification (APNs) tokens** — used only to deliver background
  notifications and Live Activities through Apple's push service. A managed
  relay keeps the device token for the active pairing for up to 90 days (and
  refreshes it while the subscription is active). It is removed when you unpair,
  when Apple invalidates it, or when the registration expires.
- **Managed notification payloads** — notification text, commands, project paths,
  and routing fields are AES-GCM encrypted on the Mac and decrypted by Leash's
  iPhone notification service extension. The relay and push provider see only
  ciphertext and an opaque room identifier. Managed Live Activity pushes carry
  generic presentation state such as pending count, progress, and an opaque
  response identifier.
- **Optional Account & Key Sync** uses Sign in with Apple. We request no name or
  email. The service stores the opaque Apple account identifier, registered
  device identifiers and public encryption keys, and encrypted key backups to
  link your devices and restore pairings.

## What we do NOT do

- We do **not** use third-party analytics, advertising, or tracking SDKs.
- We do **not** track you across apps or websites.
- We do **not** sell or share your data.
- The relay does **not** store readable message content; it forwards encrypted
  frames and stores APNs routing data plus unreadable managed-event ciphertext
  needed for delivery and offline catch-up.

## Data retention & deletion

- Local history and settings live on your device. Delete them at any time by
  unpairing/wiping in the app or by deleting the app.
- Managed-event ciphertext is removed when the phone acknowledges it or after
  7 days, whichever comes first.
- Relay traffic is transient (forwarded, not persisted as readable data). Managed
  push routing tokens expire after at most 90 days unless your device refreshes
  its registration, and unpairing requests immediate deletion.
- In Leash, open **Settings → Account & Key Sync → Delete Account** to delete
  the account record, registered device records, and encrypted key backups.

## Subscriptions

Leash offers an optional paid subscription that unlocks off-network responses
and control, Live Activities, and the live session mirror. Purchases are processed
by **Apple** through the App Store; we do not receive your payment details.
Subscriptions are managed in your Apple ID settings.

## Children

Leash is a developer tool and is not directed at children under 13.

## Contact

Questions about this policy: **adrianpmcgee@gmail.com**

## Changes

We may update this policy; material changes will be reflected by the "Last
updated" date above.
