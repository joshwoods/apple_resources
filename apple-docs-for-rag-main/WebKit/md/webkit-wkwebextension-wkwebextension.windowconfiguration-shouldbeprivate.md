

- WebKit
- WKWebExtension
- WKWebExtension.WindowConfiguration
-  shouldBePrivate 

Instance Property

# shouldBePrivate

Indicates whether the window should be private.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var shouldBePrivate: Bool { get }
```

## Discussion

Note

To ensure proper isolation between private and non-private data, web views associated with private data must use a different WKUserContentController. Likewise, to be identified as a private web view and to ensure that cookies and other website data is not shared, private web views must be configured to use a non-persistent WKWebsiteDataStore.

