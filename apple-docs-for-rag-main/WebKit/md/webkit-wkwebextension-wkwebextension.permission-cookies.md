

- WebKit
- WKWebExtension
- WKWebExtension.Permission
-  cookies 

Type Property

# cookies

A request for access to the `browser.cookies` APIs.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
nonisolated
static let cookies: WKWebExtension.Permission
```

## See Also

### Constants

static let activeTab: WKWebExtension.Permission

A request indicating that when a person interacts with the extension, the system grants extra permissions for the active tab only.

static let alarms: WKWebExtension.Permission

A request for access to the `browser.alarms` APIs.

static let clipboardWrite: WKWebExtension.Permission

A request for access to write to the clipboard.

static let contextMenus: WKWebExtension.Permission

A request for access to the `browser.contextMenus` APIs.

static let declarativeNetRequest: WKWebExtension.Permission

A request for access to the `browser.declarativeNetRequest` APIs.

static let declarativeNetRequestFeedback: WKWebExtension.Permission

A request for access to the `browser.declarativeNetRequest` APIs with extra information on matched rules.

static let declarativeNetRequestWithHostAccess: WKWebExtension.Permission

A request for access to the `browser.declarativeNetRequest` APIs with the ability to modify or redirect requests.

static let menus: WKWebExtension.Permission

A request for access to the `browser.menus` APIs.

static let nativeMessaging: WKWebExtension.Permission

A request for access to send messages to the app extension bundle.

static let scripting: WKWebExtension.Permission

A request for access to the `browser.scripting` APIs.

static let storage: WKWebExtension.Permission

A request for access to the `browser.storage` APIs.

static let tabs: WKWebExtension.Permission

A request for access to extra information on the `browser.tabs` APIs.

static let unlimitedStorage: WKWebExtension.Permission

A request for access to an unlimited quota on the `browser.storage.local` APIs.

static let webNavigation: WKWebExtension.Permission

A request for access to the `browser.webNavigation` APIs.

static let webRequest: WKWebExtension.Permission

A request for access to the `browser.webRequest` APIs.

