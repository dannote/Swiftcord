<p align=center><image src="https://raw.githubusercontent.com/SwiftcordApp/.github/main/res/swiftcord_new_icon.png" height="256" /></p>

<h1 align="center">Swiftcord</h1>

<p align="center">Native Discord client for macOS built in Swift</p>

> [!NOTE]
> This is an actively maintained fork of [SwiftcordApp/Swiftcord](https://github.com/SwiftcordApp/Swiftcord), incorporating fixes from the community and keeping the client functional with the latest Discord API changes.

[![](https://github.com/SwiftcordApp/.github/blob/main/res/hero.webp?raw=true)](https://github.com/SwiftcordApp/.github/blob/main/res/swiftcord-promo.mov?raw=true)

---

## Changes from upstream

**Critical fixes:**
- ✅ Gateway compatibility restored — login no longer hangs (updated client parity, capabilities, and DecodeThrowable handling)
- ✅ Builds on Xcode 16+ (updated Sentry, Lottie, and other dependencies)

**Features from [SwiftInstitute/Swiftcord](https://github.com/SwiftInstitute/Swiftcord):**
- Display name support
- Read/unread state management (manual ack, read on send, mark as unread)
- Context menus for guilds and channels
- Message scroll fixes (reversed list, scroll to unread, scroll to reply)
- 100+ guilds fix for Nitro users
- Font scaling / text size settings
- Settings UI redesign
- Image lightbox
- Liquid Glass UI for macOS 26 (Tahoe)
- DMG builder script

**Additional improvements:**
- Native macOS notifications for new messages
- Bot/webhook badge text visibility in light mode
- Russian localization fixes
- Compiler type-check fix for StickerPackView

Powered by [DiscordKit](https://github.com/dannote/DiscordKit) (forked with updated Gateway protocol support).

---

## Building from source

**Requirements:** macOS 12+ and Xcode 16+

```bash
git clone https://github.com/dannote/Swiftcord.git
cd Swiftcord
open Swiftcord.xcodeproj
```

Build and run the `Swiftcord` scheme.

---

## FAQ

<details>
  <summary><b>Will I get banned for using Swiftcord?</b></summary>
  Nobody really knows Discord's official stance on unofficial clients.
  Hundreds of people have been using Swiftcord for a while with no reported bans.
  The client identifies as the official Discord desktop client.
  <br><br>
  <i>Use at your own risk, preferably with an alt account first.</i>
</details>

<details>
  <summary><b>The app won't open / macOS says it's damaged</b></summary>
  If you build from source, the app is ad-hoc signed. On some macOS versions you may need to:

  ```bash
  xattr -cr /path/to/Swiftcord.app
  ```
</details>

---

## Copyright Notice

Copyright (c) 2023 Vincent Kwok & Swiftcord Contributors

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You can find a copy of the GNU General Public License v3 in LICENSE or https://www.gnu.org/licenses/.
