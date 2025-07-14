

- WebKit
- WKWebViewConfiguration
-  userContentController 

Instance Property

# userContentController

The object that coordinates interactions between your app’s native code and the webpage’s scripts and other content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var userContentController: WKUserContentController { get set }
```

## See Also

### Configuring the web view’s behavior

var websiteDataStore: WKWebsiteDataStore

The object you use to get and set the site’s cookies and to track the cached data objects.

var processPool: WKProcessPool

The object that coordinates the processes the web view uses to render its web content and execute scripts.

var applicationNameForUserAgent: String?

The app name that appears in the user agent string.

var limitsNavigationsToAppBoundDomains: Bool

A Boolean value that indicates whether the web view limits navigation to pages within the app’s domain.

var upgradeKnownHostsToHTTPS: Bool

A Boolean value that indicates whether the web view should automatically upgrade supported HTTP requests to HTTPS.

