ASTRAY FOR CHROME

# Your assistant. Your browser tabs.

Read a page, fill a form, or pick up a task in Chrome. Browser Bridge connects the tabs you choose to Astray on your Mac.

Version 0.3.3 was submitted to the Chrome Web Store on September 8, 2026, replacing the canceled 0.3.2 review. The dashboard confirmed that it is pending review. The Store installation button will be enabled in an Astray update after publication is verified. Existing users can continue using the development extension through Astray Settings.

## Get connected

**Version 0.3.3 with the matching Mac app:** install the extension and sign in to Astray on the same Mac. The connection is prepared automatically, and the popup shows your Astray account. The extension uses the Mac app's login session. Stop pauses automatic reconnection until you resume access; signing out disconnects it. The extension is pending review, and account display and automatic setup require a compatible Mac app update. The instructions below also support older companion apps.

- **Install Astray for Mac.** Requires macOS 14 or later and Google Chrome 125 or later. Keep Astray in Applications.
- **Prepare Chrome in Astray.** Open Settings → Chrome tabs. Astray installs the local connection used by the extension. Keep Apps & desktop enabled on the Mac whose tabs you want to use.
- **Add Browser Bridge to Chrome.** Once the store release is available, use the Chrome Web Store installation button in Astray. Then open the extension to check its status.
- **Start a task in Astray.** Choose a tab through your assistant. Use Stop in Astray whenever you want to end control.

[Download Astray for Mac ↗](https://github.com/walnut-computing/astray-releases/releases/latest)

## What the extension can access

Astray can list open tab titles and URLs. For selected tabs, it can read page content, take screenshots, click, type, scroll, and navigate. Results pass through the local app and may reach your workspace and AI provider for your requested task. [Read the browser privacy policy.](https://github.com/walnut-computing/astray-releases/blob/main/docs/browser-privacy.md)

## Connection help

**Checking the account connection:** With a compatible Mac app, sign in and enable Apps & desktop, then open the extension popup. It should show the account signed in to Astray, which may differ from your Chrome profile. Ask Astray to read the heading of `https://example.com`, then use Stop and verify browser control ends. Sign out of Astray and verify the popup disconnects and clears the account display. The extension has no separate sign-up or purchase.

**Companion app updates:** The extension submission did not deploy a Mac app update. The tab-recovery and readonly-waiting client fixes also require an updated Astray app. If you use a persistent JavaScript session, restart it after updating the app.

**App versions without the Store button:** Install Astray in Applications, then run the following once in Terminal to prepare its local connection for the Store extension:

```sh
/Applications/Astray.app/Contents/MacOS/Astray --install-browser-host iipkednacffnnbnfoijgdoclecjcpmcc
```

Open Astray and enable Apps & desktop. After approval, install [Astray Browser Bridge from the Chrome Web Store](https://chromewebstore.google.com/detail/iipkednacffnnbnfoijgdoclecjcpmcc). The Store page is not available for installation while review is pending.

**“Open Astray to connect”:** Open the Astray app on this Mac. In Settings, complete Chrome setup. If you moved the app, run setup again to update its local connection.

**“Waiting for Astray”:** Start a browser task in Astray. The extension connects when the app's browser service is active. You can also choose Reconnect to Astray in the extension.

**Two Chrome profiles:** Use Browser Bridge in one Chrome profile at a time on this Mac. Each browser service accepts one connected profile.

**Chrome shows a debugging message:** Browser Bridge uses Chrome's debugger permission to inspect and interact with the selected page. Use Stop in Astray to end control. Protected Chrome pages and the Chrome Web Store cannot be automated by the extension.

For help, email [yechansub@gmail.com](mailto:yechansub@gmail.com) with your Astray version, Chrome version, and the connection status shown in the popup. Please do not send passwords, cookies, private page contents, or authentication tokens.
