# FW Downloader Manager

**A fast, free download manager for Windows, with segmented downloads, video & playlist support, queues, a scheduler and a browser extension.**

**Version 1.4.16** · Windows · 7 interface languages · Free to use · Closed source

[Download](#download) · [Features](#features) · [Screenshots](#screenshots) · [Installation](#installation) · [How to Use](#how-to-use) · [Languages](#supported-languages) · [Privacy](#privacy) · [Support](#support--contact)

---

## Project Overview

**FW Downloader Manager** is a desktop download manager built to make downloading files, batches of links, videos and playlists simple and reliable. It splits files into multiple parallel connections, resumes interrupted downloads, organizes everything into categories, queues and groups, and can send videos directly from your browser through its companion extension.

> **Note:** This repository hosts the **official releases, documentation and issue tracking** for FW Downloader Manager. The application itself is **closed-source**; no source code is published here.

---

## Features

### Downloading

- **Segmented downloads** with up to **32 connections per download** (configurable; default set in *Options → Downloads*).
- **Pause and resume**, including after closing the program, when the server supports resuming. The *Check* button in the Add dialog tells you whether a file can be resumed.
- **Per-download controls:** category, queue, description, referer, number of connections and a speed limit for that download only.
- **Duplicate protection:** adding a link that is already in the list (and unfinished) reopens the existing download instead of creating a copy.
- **Safe file handling:** a finished HTTP download will not overwrite an existing file if a late name collision happens.

### Batch & Site Grabber

- **Batch download:** paste a list of links (one per line) or add them from the clipboard.
- **Numbered files:** generate links from a pattern such as `https://example.com/img_*.jpg`, with a *From / To* range and optional leading zeros (up to about 5,000 files at a time).
- **Site grabber:** read a web page, list the files linked from it, filter by type (Images, Video, Music, Compressed, Documents, Programs, General) or by name, then add only what you select.

### Videos & Playlists

- Download videos and **entire playlists** using **yt-dlp**.
- Choose **Best available, 1080p, 720p, 480p, 360p, 240p, 144p, or Audio only**.
- **MP3 extraction** with selectable bitrate: 128, 160, 192, 256 or 320 kbps (requires `ffmpeg`).
- Optional **subtitle download**, including auto-generated subtitles, saved as side files.
- A **Best available quality** fallback when a site's format list cannot be read.

### Browser Extension

- A **Download this video** button over videos in Chromium-based browsers: **Chrome, Edge, Brave, Chromium, Opera and Vivaldi**.
- Pick a quality in the browser, then **review and confirm** in the program's *Download file information* window. Nothing starts until you press *Start download* or *Download later*.
- Download links clicked in the browser are intercepted and sent to the program instead of the browser's own downloader.
- Can **launch the program automatically** if it is closed.
- Built-in **browser manager** (*Options → Browser*) showing detected browsers and the extension status of each.
- The extension communicates with a **local service running on your own computer**.

### Organization

- **Categories:** Compressed, Documents, Music, Programs, Video, Images and General, with optional per-category save folders.
- **Queues:** run files one after another with a configurable number of simultaneous downloads (1–20).
- **Groups:** gather an album, a course or a playlist into one collapsible row with combined size, progress, speed, time left and finished/active/failed counts.
- **Search and sort** the download list; show or hide table columns.
- **Import / export** your list (`.ezl`, `.json`, `.txt`), including groups.

### Control & Automation

- **Scheduler:** start and stop a chosen queue at set times.
- **Auto shutdown:** turn the computer off when a queue finishes, or once when all downloads are done, with a grace period to cancel.
- **Speed limiter:** a global limit plus an optional per-download limit.
- **Proxy support** in *Options → Downloads*.
- **System tray:** closing the window hides the program to the tray so downloads keep running; quit from the tray menu.
- **Start with Windows** in the background (can be turned off in Options).
- **Single instance:** launching it again brings the running copy forward.

### Interface

- **7 themes:** Dark, Light, Obsidian, Deep Ocean, Twilight, Black and Light Gray.
- **Interface scaling** from 90% to 175%.
- **7 interface languages** with right-to-left support for Arabic.
- A progress window per download with a connections map and per-connection table.

---

## Screenshots

### Main Window

<div align="center">
  <img src="docs/screenshots/photo_1_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_2_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_3_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_4_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_5_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_6_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_7_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_8_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_9_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_10_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_11_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_12_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_13_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_14_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_15_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_16_2026-11-04_20-22-06.jpg" alt="Main window with download list, groups and sidebar" width="85%">
  <img src="docs/screenshots/photo_2026-11-05_01-20-08.jpg" alt="Main window with download list, groups and sidebar" width="85%">
</div>

### Adding Downloads

| Add URL | Batch Download | Site Grabber |
| --- | --- | --- |
| <img src="docs/screenshots/add-url.png" alt="New download dialog" width="100%"> | <img src="docs/screenshots/batch.png" alt="Batch download dialog" width="100%"> | <img src="docs/screenshots/grabber.png" alt="Site grabber" width="100%"> |

### Video & Browser Extension

| Video / Playlist | Browser Options | Extension Button |
| --- | --- | --- |
| <img src="docs/screenshots/video.png" alt="Video and playlist dialog" width="100%"> | <img src="docs/screenshots/browser-options.png" alt="Options, Browser tab" width="100%"> | <img src="docs/screenshots/browser-button.png" alt="Extension button on a sample player" width="100%"> |

<div align="center">
  <img src="docs/screenshots/browser-confirm.png" alt="Download file information window" width="55%">
  <p><sub>Download file information window: nothing starts until you confirm.</sub></p>
</div>

### Organization & Control

| Groups | Queues | Progress Window |
| --- | --- | --- |
| <img src="docs/screenshots/groups.png" alt="Groups" width="100%"> | <img src="docs/screenshots/queues.png" alt="Queues" width="100%"> | <img src="docs/screenshots/details.png" alt="Progress window" width="100%"> |

| Scheduler | Speed Limiter | Options |
| --- | --- | --- |
| <img src="docs/screenshots/scheduler.png" alt="Scheduler" width="100%"> | <img src="docs/screenshots/limiter.png" alt="Speed limiter" width="100%"> | <img src="docs/screenshots/options.png" alt="Options" width="100%"> |

### Themes

<div align="center">
  <img src="docs/screenshots/photo_2_2026-11-04_20-22-06.jpg" alt="Available themes" width="85%">
</div>

> The screenshots use example file names and values only. The extension preview was captured on a local sample player, not a real video site.

---

## Installation

### Requirements

- **Windows** (the release is built for Windows).
- An internet connection for downloading.
- **Optional, for the browser extension:** a Chromium-based browser (Chrome, Edge, Brave, Chromium, Opera or Vivaldi).

### Install with Setup.exe

1. Open the [Download section](#download) and download **Setup.exe** from the latest release.
2. Run **Setup.exe** and follow the installer (built with Inno Setup).
3. Launch **FW Downloader Manager** when the installer finishes, or later from the Start menu or desktop shortcut if you chose to create one.
4. *(Optional)* Install the browser extension; see [Installing the Browser Extension](#installing-the-browser-extension).

> If Windows SmartScreen warns about an unrecognized publisher, make sure you downloaded the file from this repository's official Releases page before choosing to continue.

By default, the program starts with Windows in the background (in the system tray). You can turn this off in **Options → General**. Settings and the download list are stored in the `.fw_downloader_manager` folder inside your user folder.

### Extra Components for Video Downloads

Most features need nothing else. Two video-related components are worth knowing about:

| Component | What it is used for | Do you need to install it? |
| --- | --- | --- |
| **ffmpeg** | Merging separate video and audio streams, and extracting MP3 audio | Included with the application — no separate installation required., then for one in your `PATH`. If the dialog warns that ffmpeg is missing, install it and add it to your `PATH`. |
| **Node.js 22+** or **Deno 2.3+** | Reading formats from sites that use JavaScript challenges (for example YouTube) | **Not bundled.** The program detects a copy on your `PATH`. Install one only if such a site fails to list its formats. |

Regular file downloads, batches, the site grabber, queues and the scheduler do not need either component.

---

## How to Use

### Quick Start

1. Click **Add URL** in the top bar, or press <kbd>Ctrl</kbd>+<kbd>N</kbd>.
2. Paste the file link. The program suggests a file name and save folder.
3. Click **Start Download** to begin now, or **Download Later** to add it to the list.
4. Follow progress in the table. Double-click an unfinished download to open its progress window, or a finished one to open the file.

### Batch Downloads

Press <kbd>Ctrl</kbd>+<kbd>B</kbd> and choose **Links list** (one link per line) or **Numbered files** (use `*` as the number placeholder). Pick a queue and save folder, optionally give the batch a group name, then choose **Add only** or **Add and start**.

### Site Grabber

**Tasks → Run site grabber…**, enter the page address, press **Grab**, filter the results by type or name, select what you want, then press **Add selected**.

### Videos & Playlists

**Tasks → Download a video / playlist…**, paste the address and press **Fetch**. Choose a quality, tick the items you want, pick the save folder, queue and group, then press **Download selected**.

### Installing the Browser Extension

1. Open **Options → Browser**. Detected browsers and their extension status are listed.
2. On your browser's row, press **Copy path and open**. The program prepares the extension folder, copies its path and opens that browser's extensions page.
3. On the extensions page, turn on **Developer mode** and click **Load unpacked**.
4. Paste the copied path (<kbd>Ctrl</kbd>+<kbd>V</kbd>) into the folder picker, press <kbd>Enter</kbd> and select the folder.
5. Return to the program and press **Refresh browser status**.

Then reload any video page, hover the round button in the video's corner, choose a quality and confirm the download in the program.

> **Do not share the extension folder with anyone; it contains a connection token specific to your installation.**

### Queues, Scheduler & Speed Limit

- **Queues:** right-click *Queues* in the sidebar → *New queue…*. Use **Start Queue / Stop Queue** to run or stop it.
- **Scheduler:** click **Scheduler** in the toolbar, enable it, choose a queue and a start time (and optionally a stop time or shutdown when finished).
- **Speed limiter:** click **Limiter** in the toolbar, or set it in *Options → Speed*.

### Keyboard Shortcuts

| Shortcut | Action |
| --- | --- |
| <kbd>Ctrl</kbd>+<kbd>N</kbd> | New download |
| <kbd>Ctrl</kbd>+<kbd>B</kbd> | Batch download |
| <kbd>Ctrl</kbd>+<kbd>G</kbd> | New group from selection |
| <kbd>Ctrl</kbd>+<kbd>A</kbd> | Select all downloads |
| <kbd>Ctrl</kbd>+<kbd>O</kbd> | Options |
| <kbd>Ctrl</kbd>+<kbd>=</kbd> / <kbd>Ctrl</kbd>+<kbd>-</kbd> / <kbd>Ctrl</kbd>+<kbd>0</kbd> | Larger / smaller / reset interface size |
| <kbd>Ctrl</kbd>+<kbd>Q</kbd> | Hide to tray (or exit when no system tray is available) |
| <kbd>Delete</kbd> | Remove selection from the list |
| <kbd>←</kbd> / <kbd>→</kbd> | Collapse / expand a group |

### Good to Know

- **Closing the window does not quit the program.** Use **Exit** from the tray icon menu to fully quit.
- **Limits:** the program has **no torrent or `magnet:` support**. It does **not** bypass DRM, mandatory sign-in or site restrictions. Video support depends on what yt-dlp supports for each site.
- **Sign-in prompts:** if a video site asks you to sign in or verify, sign in using the same browser and start the download from the extension.
- **Firefox** is detected but **not supported**: the extension is built for Chromium-based browsers only.

---

## Supported Languages

The interface can be switched from **View → Language** (or *Options → General*) and applies immediately.

| Language | Code |
| --- | --- |
| English | `en` |
| العربية (Arabic, right-to-left) | `ar` |
| Français (French) | `fr` |
| Español (Spanish) | `es` |
| Português (Brasil) | `pt_BR` |
| Deutsch (German) | `de` |
| Polski (Polish) | `pl` |

---

## Download

Get the latest version from **GitHub Releases**:

<div align="center">
  <h3><a href="https://github.com/FouadWre-Dev/FW-Downloader-Manager/releases/latest">Download the Latest Release</a></h3>
  <p><a href="https://github.com/FouadWre-Dev/FW-Downloader-Manager/releases">View All Releases</a></p>
</div>

> Always download from the official Releases page of this repository.

---

## Privacy

- The browser extension communicates only with a service running **locally on your computer** (default port `6879`, changeable in Options).
- Cookies, when needed for a video, are sent only to that local service and are **not** saved in your download list.

### Pseudonymous Usage Statistics

To count installs and improve the app, the program can send encrypted statistics tied to a **random installation ID** (generated locally, not derived from your name or hardware).

Because this ID stays the same on your installation, these statistics are **pseudonymous**, not fully anonymous.

**What is sent:**

- The random installation ID.
- The app version.
- Your operating system name and interface language.
- The number of completed downloads.
- A sanitized crash/error description (error type and the program's own source file and line numbers; at most 3 per session).

**What is never sent:**

- Download links.
- File names.
- Folder paths.
- User names or other personal data.

**Your control:**

A notice explains this on first run, and nothing is sent before you have seen it. You can turn statistics off at any time in **Options → General** using the option **Send anonymous usage statistics**.

This is the exact option label shown in the program; despite the label, the statistics are pseudonymous as explained above. Choosing "off" means nothing is ever sent.

---

## Support & Contact

Questions, bug reports or suggestions?

- **Bugs & feature requests:** open an issue in this repository's **Issues** tab. Please include your program version, Windows version and, for video problems, your browser and the site involved.
- **Telegram:** [t.me/DevFouad](https://t.me/DevFouad)
- **Facebook:** [facebook.com/hakimDvloper](https://www.facebook.com/hakimDvloper)
- **Built-in guide:** *About → Program Guide* inside the program.

---

## Developer

**Fouad Wre**, developer and maintainer of FW Downloader Manager.

If you enjoy the program and want to support its continued development, you can find the support option in the program's **About** window.

---

## License

FW Downloader Manager is **closed-source software**, free to use. The source code is not published in this repository.

---

<div align="center">
  Made with care by **Fouad Wre**
</div>
