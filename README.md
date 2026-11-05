<div align="center">

# Dami

**Your mail stays, even after the server deletes it**

A Windows app that keeps your IMAP and POP3 mail on your own PC, permanently.

[**Download the latest version**](https://github.com/gaurilabs/dami/releases/latest)

</div>

![Dami mail view](docs/images/main-dark.png)

## Why Dami?

Mail you deleted because your mailbox was full, mail that expired under a server retention policy, mail you lost access to when you left a job or a service shut down: all of it is hard to get back.

Dami keeps an exact copy of your mail on your PC. **Mail deleted from the server stays in Dami, and Dami never deletes or changes anything on the server.**

## Features

### Deleted mail stays

Mail that disappears from the server is kept and marked `Server-deleted`. Each account has a `Deleted from server` folder that gathers it in one place.

![Viewing mail deleted from the server](docs/images/server-deleted.png)

### Read-only on the server

- IMAP connects in read-only mode and never marks mail as read.
- POP3 never uses the command that deletes mail from the server.
- Mail is saved exactly as received, as `.eml` files.

### Fast full-text search

Search subjects, message bodies, and attachment names across every account and date range at once. Partial-word matching works in any language, including Korean, Chinese, and Japanese.

![Mail search](docs/images/search.png)

### Scheduled backups and status

Set a backup schedule for each account. Dami keeps running in the system tray after you close the window, and shows overall status and an activity log at a glance.

![Backup status](docs/images/dashboard.png)

### Integrity checks

Dami verifies archived files against their SHA-256 hashes. It never fixes or deletes anything automatically: if a problem is found, you choose whether to restore from a copy or download the message from the server again.

![Integrity check](docs/images/integrity.png)

### Import and export

- **Import:** EML, MSG, MBOX, Thunderbird local folders, Gmail Takeout, Outlook PST and OST
- **Export:** EML (exact original), MBOX

Bring the archives from your previous mail apps together in one place.

### Available in 9 languages

English, 한국어, 简体中文, 繁體中文, 日本語, Español, Deutsch, Français, Português (Brasil)

Dami follows your Windows language and falls back to English if that language isn't supported. To change it, go to **Settings → Display**. The new language applies when you save, and Dami restarts automatically.

### And more

- Dark and light themes
- Scripts in mail are always blocked, and external images are blocked by default
- Move your archive to another drive
- Automatic update checks and updates

![Light theme](docs/images/main-light.png)

## Installation

1. Download `Dami_<version>_win-x64_setup.exe` from [Releases](https://github.com/gaurilabs/dami/releases/latest).
2. Run the installer. Administrator rights aren't required.
3. Start Dami and add your mail account.

> The installer isn't code-signed, so Windows SmartScreen may show a warning. If it does, select **More info → Run anyway**.

When a new version is available, Dami lets you know and updates itself once you approve.

### System requirements

| Item | Requirement |
|------|-------------|
| Operating system | Windows 10 version 1809 or later, Windows 11 (x64) |
| Runtime | Included in the installer |
| Mail body display | WebView2 Runtime (already installed on most Windows 10 and 11 PCs) |

## Good to know

- **Connecting accounts:** Use an app password from your mail provider. OAuth sign-in isn't supported.
- **Passwords:** Encrypted with DPAPI, which ties them to your Windows user account.
- **Data location:** Stored in `%LOCALAPPDATA%\Dami`. You can move it in Settings.
- **Uninstalling keeps your mail:** Your archive and settings aren't removed when you uninstall.
- **Network connections:** Dami connects only to your mail servers and to GitHub to check for new versions. You can turn off automatic update checks in Settings.

## Support

Please report bugs and share suggestions in [Issues](https://github.com/gaurilabs/dami/issues).

## License

Dami is distributed under the MIT License. This repository is for releases only; the source code is not public.

---

<sub>All accounts, people, and messages shown in the screenshots are fictional.</sub>

<sub>Copyright © 2026 GauriLab. All rights reserved.</sub>
