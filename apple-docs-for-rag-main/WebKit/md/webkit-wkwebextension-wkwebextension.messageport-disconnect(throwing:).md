

- WebKit
- WKWebExtension
- WKWebExtension.MessagePort
-  disconnect(throwing:) 

Instance Method

# disconnect(throwing:)

Disconnects the port, terminating all further messages with an optional error.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func disconnect(throwing error: (any Error)?)
```

## Parameters 

`error`  

An optional error indicating the reason for disconnection.

