

- WebKit
- WKWebExtensionContext
-  isInspectable 

Instance Property

# isInspectable

Determines whether Web Inspector can inspect the WKWebView instances for this context.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var isInspectable: Bool { get set }
```

## Discussion

A context can control multiple WKWebView instances, from the background content, to the popover.

You should set this to `YES` when needed for debugging purposes. The default value is `NO`.

