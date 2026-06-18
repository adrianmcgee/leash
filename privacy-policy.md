# Leash — Privacy Policy

_Last updated: June 18, 2026_

Leash ("the app") connects your iPhone, Apple Watch, and Mac so you can see and
respond to your AI coding agent (Claude Code and compatible CLIs) remotely. This
policy explains what data Leash handles and how.

**Summary: Leash is built to be zero-knowledge. Your data stays on your devices.
We do not run an analytics server, we do not sell data, and we cannot read the
content that passes between your phone and your Mac.**

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
- **Pairing secrets** are stored in the Apple **Keychain** on your devices and
  are never transmitted to us.
- **Settings, paired-Mac records, and recent-notification history** are stored
  **locally** on your device (and shared with the Leash widget via an app group).
- **Apple Push Notification (APNs) device token** — used only to deliver
  background notifications via Apple's push service. Push payloads do not contain
  your private content beyond what is needed to display a notification, and are
  delivered through Apple.

## What we do NOT do

- We do **not** use third-party analytics, advertising, or tracking SDKs.
- We do **not** track you across apps or websites.
- We do **not** sell or share your data.
- The relay does **not** store your message content; it forwards encrypted frames
  between your paired devices and holds nothing it can read.

## Data retention & deletion

- Local history and settings live on your device. Delete them at any time by
  unpairing/wiping in the app or by deleting the app.
- Relay traffic is transient (forwarded, not persisted as readable data).

## Subscriptions

Leash offers an optional paid subscription that unlocks remote access over the
relay, push notifications, and the live session mirror. Purchases are processed
by **Apple** through the App Store; we do not receive your payment details.
Subscriptions are managed in your Apple ID settings.

## Children

Leash is a developer tool and is not directed at children under 13.

## Contact

Questions about this policy: **adrianpmcgee@gmail.com**

## Changes

We may update this policy; material changes will be reflected by the "Last
updated" date above.
