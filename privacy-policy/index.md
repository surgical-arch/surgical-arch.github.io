# Privacy Policy for PRISM

* Effective Date: 2026. 01. 23

1. Information Collection PRISM does not collect, track, or transmit any personally identifiable information (PII) or sensitive user data to external servers. We do not require account creation or login to use the extension.

2. Data Processing

- All data processed by PRISM occurs exclusively on the user's local device. The extension analyzes text, URLs to provide contextual evaluation and summary of media content within the browser. This processing is transient and is used only to perform the extension's core functionality.

3. Data Storage
   
- PRISM does not store your data on our servers. Any settings or preferences you save are stored locally on your device using Chrome's local storage API. These settings are deleted if you uninstall the extension.

4. Data Sharing and Disclosure
   
- We do not sell, trade, or share any user data with third parties. Since we do not collect any data, there is no information to disclose to law enforcement, advertisers, or other third-party entities.

5. Permissions Disclosure PRISM requests only the minimum permissions necessary to function:

- storage: To save your personal settings locally.

- activeTab/tabs: To analyze the content of the page you are currently viewing.

- activeTab
  - Reason: Required to temporarily access the currently active tab when the user clicks the extension icon or interacts with it.
  - Details: Typically used to read information from or manipulate the page the user is currently viewing, primarily for the popup (popup.html).
- storage
  - Reason: Required to save and retrieve settings and state information locally.
  - Details: chrome.storage.local to manage data such as API keys (keys), extension enable status (extensionEnabled), font size preferences (fontSize), and the selected AI provider (activeProvider).
- scripting
  - Reason: Required to dynamically inject JavaScript code into web pages.
  - Details: Used in to immediately execute (inject) into already open YouTube tabs when the extension is installed or updated, ensuring the extension works immediately without requiring a page refresh.

- host_permissions (Host Access Permissions)
  - https://*.youtube.com/*
  - Required to access all YouTube pages to read data and display the UI. Allows to extract metadata (DOM scraping) such as video titles, channel names, and URLs from YouTube pages. Enables the insertion of the analysis result window (Shadow DOM) directly into the YouTube interface for the user to see.
  - https://generativelanguage.googleapis.com/*
  - Required to communicate with Google's Gemini AI API servers. send prompts via the fetch function to the Gemini API and receive analysis results. (This allows direct requests to the AI server bypassing CORS issues).

6. User Rights As no data is collected on our servers, users have full control over their data locally. You can stop all data processing at any time by disabling or removing the extension from your browser.

7. Contact Us If you have any questions, please contact us at: surgical.arch@gmail.com
