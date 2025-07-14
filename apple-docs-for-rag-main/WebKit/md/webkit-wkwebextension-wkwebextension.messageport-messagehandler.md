

- WebKit
- WKWebExtension
- WKWebExtension.MessagePort
-  messageHandler 

Instance Property

# messageHandler

The block to be executed when a message is received from the web extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var messageHandler: ((Any?, (any Error)?) -> Void)? { get set }
```

## Discussion

An optional block to be invoked when a message is received, taking two parameters: the message and an optional error.

