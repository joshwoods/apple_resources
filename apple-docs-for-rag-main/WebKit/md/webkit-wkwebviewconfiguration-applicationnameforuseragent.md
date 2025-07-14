

- WebKit
- WKWebViewConfiguration
-  applicationNameForUserAgent 

Instance Property

# applicationNameForUserAgent

The app name that appears in the user agent string.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
var applicationNameForUserAgent: String? { get set }
```

## See Also

### Configuring the web view’s behavior

var websiteDataStore: WKWebsiteDataStore

The object you use to get and set the site’s cookies and to track the cached data objects.

var userContentController: WKUserContentController

The object that coordinates interactions between your app’s native code and the webpage’s scripts and other content.

var processPool: WKProcessPool

The object that coordinates the processes the web view uses to render its web content and execute scripts.

var limitsNavigationsToAppBoundDomains: Bool

A Boolean value that indicates whether the web view limits navigation to pages within the app’s domain.

var upgradeKnownHostsToHTTPS: Bool

A Boolean value that indicates whether the web view should automatically upgrade supported HTTP requests to HTTPS.

