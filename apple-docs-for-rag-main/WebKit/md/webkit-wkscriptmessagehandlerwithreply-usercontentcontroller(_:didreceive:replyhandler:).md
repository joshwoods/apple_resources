

- WebKit
- WKScriptMessageHandlerWithReply
-  userContentController(\_:didReceive:replyHandler:) 

Instance Method

# userContentController(\_:didReceive:replyHandler:)

Tells the handler that a webpage sent a script message that included a reply.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
func userContentController(
    _ userContentController: WKUserContentController,
    didReceive message: WKScriptMessage,
    replyHandler: @escaping @MainActor (Any?, String?) -> Void
)
```

``` source
@MainActor
func userContentController(
    _ userContentController: WKUserContentController,
    didReceive message: WKScriptMessage
) async -> (Any?, String?)
```

**Required**

## Parameters 

`userContentController`  

The user content controller that delivered the message to your handler.

`message`  

An object that contains the message details.

`replyHandler`  

A reply handler block to execute with the response to send back to the webpage. This block has no return value and takes the following parameters:

reply  
An object that contains the data to return to the webpage. Allowed types for this parameter are NSNumber, NSString, NSDate, NSArray, NSDictionary, and NSNull. Specify `nil` if an error occurred.

errorMessage  
`nil` on success, or a string that describes the error that occurred.

## Discussion

Use this method to handle a message from the webpage and provide an appropriate response.

## See Also

### Receiving Messages

class WKScriptMessage

An object that encapsulates a message sent by JavaScript code from a webpage.

