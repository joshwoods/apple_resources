

- WebKit
- WKWebExtension
- WKWebExtension.MessagePort
-  sendMessage(\_:completionHandler:) 

Instance Method

# sendMessage(\_:completionHandler:)

Sends a message to the connected web extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func sendMessage(
    _ message: Any?,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
@MainActor
func sendMessage(_ message: Any?) async throws
```

## Parameters 

`message`  

The JSON-serializable message to be sent.

`completionHandler`  

An optional block to be invoked after the message is sent, taking an optional error.

## Discussion

Note

The message must be JSON-serializable according to doc://com.apple.documentation/documentation/foundation/foundation/jsonserialization.

