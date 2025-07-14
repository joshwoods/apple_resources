

- WebKit
- WKWebExtension
- WKWebExtension.TabConfiguration
-  window 

Instance Property

# window

Indicates the window where the tab should be opened.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var window: (any WKWebExtensionWindow)? { get }
```

## Discussion

If this property is `nil`, no window was specified.

