

- WebKit
- WKWebExtension
- WKWebExtension.MessagePort
-  applicationIdentifier 

Instance Property

# applicationIdentifier

The unique identifier for the app to which this port should be connected.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var applicationIdentifier: String? { get }
```

## Discussion

This identifier is provided by the web extension and may or may not be used by the app. It’s up to the app to decide how to interpret this identifier.

