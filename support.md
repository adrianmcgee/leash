# Leash — Support

Leash puts your AI coding agent on a leash: your iPhone, Apple Watch, and Mac
stay in sync so you can approve commands, answer questions, and steer your agent
from anywhere. Works with Claude Code today, with more agents on the way.

## Getting started

1. **Install the Leash Mac app** on the Mac where you run your agent:
   [**download the DMG**](https://github.com/adrianmcgee/leash/releases/latest/download/Leash.dmg),
   drag Leash to Applications, open it, and install the hook from the app.
   _No Mac app running = no notifications._
2. **Open Leash on your iPhone** and pair:
   - **Same Wi-Fi:** your Mac is found automatically — tap Connect.
   - **Off Wi-Fi:** scan the QR code or paste the pairing link from the Mac app
     to connect over the encrypted relay.
3. Run your agent as usual. When it needs you, your phone buzzes.

## Common issues

- **No notifications when the app is closed.** Background notifications require
  push to be configured and a subscription that enables the relay/APNs path. Make
  sure the Mac app is open and you are paired.
- **"Not delivered" / can't reach the Mac off Wi-Fi.** The Mac app must be open
  and paired over the relay. Re-pair with QR or Paste Link from the Mac app.
- **Notifications on the wrong network.** On the same Wi-Fi, connection is
  automatic; some routers isolate Wi-Fi clients — try the relay path instead.
- **Snooze vs. disconnect.** Snooze pauses prompts on this phone only; your Mac
  keeps working.

## Privacy

See the [Privacy Policy](./privacy-policy.md). Leash is zero-knowledge: your
content stays on your devices, and the relay only ever sees ciphertext.

## Contact

Email **adrianpmcgee@gmail.com** with your device model, iOS/macOS version, and a
description of the issue (screenshots help).
