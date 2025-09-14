# Advanced Tool — v1.0.2

**Advanced Tool** is a lightweight, Windows-focused multi-tool — a one‑click utility that bundles a set of common system fixes and tweaks into a single app. It's ideal for power users, support technicians, and anyone who wants to quickly apply fixes and diagnostic steps without running dozens of manual commands.

> **Short pitch:** one-click fixes for common Windows problems — cleanup, networking, certificates, activation checks, and more.

---

## Features

* One-click apply of commonly used Windows fixes:

  * Flush DNS, reset network adapters, and renew IP
  * Repair Windows Update components
  * Fix common registry issues and permissions
  * Clear temporary files and compact system caches
  * Reinstall or repair root certificates
  * Reset firewall rules to defaults
  * Basic driver checks and helpful links to update drivers
* Small, portable executable — drop into any folder and run (no installer required)
* Optional CLI mode for automation and scripting
* Safety-first: each fix shows a short description and requests confirmation before making system changes
* Log file output for troubleshooting and support

---

## Screenshot

*Add a screenshot here in the `docs/screenshots/` folder and reference it in the repository.*

---

## Requirements

* Windows 10 or Windows 11 (x64 recommended)
* For some advanced repairs, administrative privileges are required. Run the tool as Administrator.
* (Optional) .NET runtime if you ship a .NET build — otherwise native EXE builds are supported.

---

## Installation

1. Download the latest release from the **Releases** page.
2. Unzip the archive into a folder of your choice.
3. Right-click the EXE and choose **Run as administrator** for full functionality.

---

## Usage

### Graphical mode

* Launch the EXE and choose the fixes you want to apply. The UI lists each action and a short description. Click **Run** to execute.


---

## Changelog — v1.0.2

* **Fixed:** Several minor bugs in the Windows Update repair sequence.
* **Improved:** Certificate reinstall routine now supports additional root store paths.
* **Added:** `--dry-run` support and more verbose logging output.
* **Updated:** UI copy and instructions for first-time users.

(See `CHANGELOG.md` for historical changelog entries.)

---

## Safety & Backups

* The tool creates restore points and backups where appropriate before modifying the system.
* If a fix could noticeably change system behavior (registry edits, firewall resets), the app will prompt for confirmation.
* Always review the list of actions before confirming.
---

## License

This project is licensed under the **MIT License** — see `LICENSE` for details.

---

## Support

If you find issues or want a new feature, please open an issue in this repository with:

* A short description of the problem
* The steps you took
* The log file (if available)

Maintainer: *The Red Wolf Team*

---

## FAQ

**Q:** Is this safe to run on production machines?

**A:** Many of the included fixes are low-risk, but some operations (firewall reset, registry edits) can change system behavior. Always run on a test machine first and keep backups.

---
