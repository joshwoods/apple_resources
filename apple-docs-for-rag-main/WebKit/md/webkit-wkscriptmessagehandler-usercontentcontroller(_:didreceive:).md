

- WebKit
- WKScriptMessageHandler
-  userContentController(\_:didReceive:) 

Instance Method

# userContentController(\_:didReceive:)

Tells the handler that a webpage sent a script message.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
func userContentController(
    _ userContentController: WKUserContentController,
    didReceive message: WKScriptMessage
)
```

**Required**

## Parameters 

`userContentController`  

The user content controller that delivered the message to your handler.

`message`  

An object that contains the message details.

## Discussion

Use this method to respond to a message sent from the webpage’s JavaScript code. Use the message parameter to get the message contents and to determine the originating web view.

## See Also

### Receiving Messages

class WKScriptMessage

An object that encapsulates a message sent by JavaScript code from a webpage.

