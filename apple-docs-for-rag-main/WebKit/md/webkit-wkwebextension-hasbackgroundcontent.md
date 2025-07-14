

- WebKit
- WKWebExtension
-  hasBackgroundContent 

Instance Property

# hasBackgroundContent

A Boolean value indicating whether the extension has background content that can run when needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var hasBackgroundContent: Bool { get }
```

## Discussion

If this property is `YES`, the extension can run in the background even when no webpages are open.

