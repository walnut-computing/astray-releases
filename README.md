# Astray for Mac

Same conversation, another Mac.

Astray connects two Macs on your local network so your existing AI conversation can work with apps, browser tabs, and an optional terminal on the other Mac.

**[Releases and downloads](https://github.com/walnut-computing/astray-releases/releases)** · **[Report a problem](https://github.com/walnut-computing/astray-releases/issues)**

> The first public release is being prepared. Downloads will appear in Releases after Apple notarization is verified.

Requires **macOS 14 or later**. One universal app supports **Apple Silicon and Intel**.

## Install

1. Download the versioned `Astray-*.zip` archive from Releases and unzip it.
2. Move `Astray.app` into **Applications** on both Macs.
3. Open Astray on both Macs while connected to the same local network.
4. Select the other Mac, click **Connect**, and enter the code shown on that Mac.
5. To use your existing Codex conversation, select **Add to Codex** on the requesting Mac and reload that MCP server in Codex.

The receiving Mac only needs Astray. Desktop control requires macOS Accessibility and Screen Recording permission on that Mac. Terminal commands and Chrome tab control have separate setup options in Settings.

## Updates

From version 0.7.0 onward, Astray includes Sparkle automatic updates. Choose **Astray → Check for Updates…**, or configure automatic checks and downloads in Settings. Finish running commands and release remote control before restarting to install.

**Updating from 0.6.0 or earlier:** quit Astray on both Macs and replace the Applications copy manually once. Re-register the Applications copy with Add to Codex if your existing registration points to an old development build. Subsequent versions can update from inside Astray.

If an MCP session was running during an update, reload it and reconnect the Macs. Updating the app does not migrate live terminal sessions or JavaScript state.

Public release archives use a timestamped Developer ID signature and Apple notarization. Sparkle verifies signed archives and the signed update feed. Every release also includes a SHA-256 checksum file for manual verification.

## About this repository

Astray is proprietary software. This public repository contains distribution files, release notes, update metadata, and support discussions. The application source is maintained separately and is not published here. Third-party license notices, including Sparkle and Node.js, are included in the app.

For bug reports, include your Astray version and macOS version, and remove private content, pairing codes, credentials, and personal data from logs or screenshots before posting.

© 2026 WalNut.
