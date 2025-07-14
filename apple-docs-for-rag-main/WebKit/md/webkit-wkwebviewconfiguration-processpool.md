

- WebKit
- WKWebViewConfiguration
-  processPool 

Instance Property

# processPool

The object that coordinates the processes the web view uses to render its web content and execute scripts.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var processPool: WKProcessPool { get set }
```

## Discussion

When it initializes a web view, WebKit either creates a new web content process in the specified pool, or uses an existing process from that pool.

## See Also

### Configuring the web view’s behavior

var websiteDataStore: WKWebsiteDataStore

The object you use to get and set the site’s cookies and to track the cached data objects.

var userContentController: WKUserContentController

The object that coordinates interactions between your app’s native code and the webpage’s scripts and other content.

var applicationNameForUserAgent: String?

The app name that appears in the user agent string.

var limitsNavigationsToAppBoundDomains: Bool

A Boolean value that indicates whether the web view limits navigation to pages within the app’s domain.

var upgradeKnownHostsToHTTPS: Bool

A Boolean value that indicates whether the web view should automatically upgrade supported HTTP requests to HTTPS.

