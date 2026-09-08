ASTRAY BROWSER BRIDGE

# Browser privacy.

Effective September 9, 2026

Astray Browser Bridge connects Chrome to the Astray app on your Mac so an assistant can work with tabs for a task you request.

This policy covers the Chrome extension and how browser information is passed to its companion app. The publisher is Astray (Chrome Web Store publisher: yechansub). Contact: [yechansub@gmail.com](mailto:yechansub@gmail.com).

## Information the extension handles

- **Astray account display (0.3.3 and matching app):** the name and, when available, email of the account signed in to Astray on this Mac, shown in the popup to identify the connection. The app supplies this over the authenticated local native connection. The extension does not receive the app's OAuth access or refresh tokens.
- **Tab information:** open tab identifiers, titles, and URLs, when Astray requests a tab list. This can reveal browsing activity. Version 0.3.7 also receives URLs, titles and visit times from Chrome's history API when recent history is requested for a task.
- **Task groups:** Chrome group identifiers and titles used to organize tabs created for a task, plus temporary session ownership and deliverable/handoff marks used for normal task cleanup. Membership in a group does not make a user tab eligible for cleanup.
- **Selected page content:** page text, accessibility and DOM information, form labels and values, links, and viewport screenshots when a task requests them. Only tabs claimed by an authorized Astray control session are inspected or controlled.
- **Task inputs and results:** text to enter, clicks, scrolling, navigation, action results, and temporary control-session identifiers necessary to carry out the task.
- **Files:** file paths explicitly supplied to a file chooser, and metadata and local file paths of media downloads started by the assistant. A chooser must belong to the controlled tab and current document. An unrelated user download is never assigned to the task by matching its URL or start time.

Depending on the pages you choose, content and screenshots may include names, email addresses, account or authentication information visible on a page, personal communications, location information, financial information, health information, or other sensitive content. The extension does not separately request geolocation or read Chrome's cookie database or saved-password vault. Password-like values are masked in structured observations where recognized; this is not a guarantee that every sensitive detail in page content or screenshots is removed.

## How information is used and shared

The extension uses this information only to provide the requested browser-assistance features and their operation and security. It communicates with the locally installed `com.astray.browser` native messaging host. The extension itself has no analytics SDK, advertising integration, or direct connection to an external data-collection server.

**The local connection does not mean the results always stay on your Mac.** The Astray app may pass the information to the workspace, connected controller, or AI service involved in your task:

- The Astray service and its infrastructure providers, currently Naver Cloud for hosting and Cloudflare for network delivery, process information carried by the hosted app.
- Members with access to the relevant Astray workspace or conversation may see browser results included in that conversation.
- Astray's built-in AI uses OpenRouter and the model provider identified by the model selected in Astray. Browser results included in the model context may be sent to both. The selected model and provider can change with your settings.
- If you connect Astray to a separate assistant or MCP client, such as ChatGPT/Codex or another client you configure, that client and its selected AI provider receive the browser results requested through it.

These recipients process information under their applicable service and privacy terms. Only connect a workspace or assistant you intend to receive the requested browser information. Astray does not sell browser data, use it for advertising, or use it to determine creditworthiness or lending eligibility.

## Storage and retention

The extension keeps connection state, account display information, tab claims, and temporary observations in memory while operating. It does not maintain a persistent browser-content database. Account display information is cleared when the native connection disconnects, including when the app signs out. Claims and debugger sessions are released when control is stopped or the native connection disconnects.

Task-session ownership and tab marks are also kept in memory. Normal task completion closes only unmarked tabs created by that session under the same control lease. Deliverable and handoff tabs and preexisting user tabs remain open. Stop, reset, and disconnect preserve tabs and remove cleanup authority. Chrome may retain the created tabs and group names after control ends; you can rename, ungroup, or close them in Chrome.

The extension stores a random extension-instance identifier in Chrome's local extension storage and opaque tab identifiers in Chrome's session storage. These support consistent browser selection and do not contain page content or login tokens. Downloaded files remain in Chrome's configured download location until you remove them. Uploading a selected file passes its content to the selected website through the browser's normal file-input flow.

The companion app, requesting client, and hosted workspace may retain conversation content, task results, and command records. These records are separate from the extension, may remain after the extension is removed, and currently have no universal automatic expiration period. AI providers and connected clients apply their own retention policies. Contact the publisher below to request access to or deletion of data held by Astray; requests may require verification of the account and workspace involved. Do not email passwords or page contents with your request.

## Your controls

Choose which tasks and tabs to use with Astray. Use **Stop** in Astray to end control. You can disable or remove the extension in Chrome's extension settings at any time. Removing it prevents further extension access but does not delete records already held by a workspace, assistant, or AI provider.

## Security and limited use

The extension uses Chrome's native messaging connection to an Astray host that checks the allowed extension origin. The app uses authenticated control sessions, and the hosted service uses HTTPS/WSS for network transport. Chrome can display a debugging notification during browser control.

Astray Browser Bridge's use and transfer of information received from Google APIs adheres to the [Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/user-data-faq), including the Limited Use requirements. Browser information is used for the disclosed user-facing task features and their necessary operation and security.

## Changes and contact

Material changes to browser-data practices will be reflected here and in the extension's disclosures. For privacy questions or requests, contact [yechansub@gmail.com](mailto:yechansub@gmail.com).
