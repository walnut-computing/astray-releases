ASTRAY FOR CHROME

# Your assistant. Your browser tabs.

Read a page, fill a form, or pick up a task in Chrome. Browser Bridge connects the tabs you choose to Astray on your Mac.

Version 0.3.1 was submitted to the Chrome Web Store on September 8, 2026 and is awaiting review. It will publish automatically after approval. The Store installation button will be enabled in an Astray update after publication. Existing users can continue using the development extension through Astray Settings.

## Get connected

- **Install Astray for Mac.** Requires macOS 14 or later and Google Chrome 125 or later. Keep Astray in Applications. 
- **Prepare Chrome in Astray.** Open Settings → Chrome tabs. Astray installs the local connection used by the extension. Keep Apps & desktop enabled on the Mac whose tabs you want to use. 
- **Add Browser Bridge to Chrome.** Once the store release is available, use the Chrome Web Store installation button in Astray. Then open the extension to check its status. 
- **Start a task in Astray.** Choose a tab through your assistant. Use Stop in Astray whenever you want to end control. 

[Download Astray for Mac ↗](https://github.com/walnut-computing/astray-releases/releases/latest) 

## What the extension can access

Astray can list open tab titles and URLs. For selected tabs, it can read page content, take screenshots, click, type, scroll, and navigate. Results pass through the local app and may reach your workspace and AI provider for your requested task. [Read the browser privacy policy.](https://github.com/walnut-computing/astray-releases/blob/main/docs/browser-privacy.md)

## Connection help

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
