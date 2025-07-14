

- WebKit
- WKWebExtension
- WKWebExtension.MessagePort
-  disconnectHandler 

Instance Property

# disconnectHandler

The block to be executed when the port disconnects.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var disconnectHandler: (((any Error)?) -> Void)? { get set }
```

## Discussion

An optional block to be invoked when the port disconnects, taking an optional error that indicates if the disconnection was caused by an error.

