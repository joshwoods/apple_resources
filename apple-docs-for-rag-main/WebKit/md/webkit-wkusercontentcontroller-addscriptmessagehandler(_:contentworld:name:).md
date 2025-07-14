

- WebKit
- WKUserContentController
-  addScriptMessageHandler(\_:contentWorld:name:) 

Instance Method

# addScriptMessageHandler(\_:contentWorld:name:)

Installs a message handler that returns a reply to your JavaScript code.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
func addScriptMessageHandler(
    _ scriptMessageHandlerWithReply: any WKScriptMessageHandlerWithReply,
    contentWorld: WKContentWorld,
    name: String
)
```

## Parameters 

`scriptMessageHandlerWithReply`  

The message handler object that implements your custom code. This object must adopt the WKScriptMessageHandlerWithReply protocol.

`contentWorld`  

The content world in which to install the message handler. Use the content world to scope your message handler to specific parts of your JavaScript code.

`name`  

The name of the message handler. This parameter must be unique within the user content controller and must not be an empty string.

The user content controller uses this parameter to define a JavaScript function for your message handler in all frames in the specified content world. The name of this function is `window.webkit.messageHandlers.``.postMessage()`, where corresponds to the value of this parameter. For example, if you specify the string `MyFunction`, the user content controller defines the `window.webkit.messageHandlers.MyFunction.postMessage()` function in JavaScript.

## Discussion

To execute your handler’s code, call the JavaScript function that this method defines. You may pass a parameter value to the method. The user content controller packages that value into an appropriate type and delivers it to your content handler’s delegate method.

## See Also

### Adding and Removing Message Handlers

func add(any WKScriptMessageHandler, name: String)

Installs a message handler that you can call from your JavaScript code.

func add(any WKScriptMessageHandler, contentWorld: WKContentWorld, name: String)

Installs a message handler that you can call from the specified content world in your JavaScript code.

func removeScriptMessageHandler(forName: String)

Uninstalls the custom message handler with the specified name from your JavaScript code.

func removeScriptMessageHandler(forName: String, contentWorld: WKContentWorld)

Uninstalls a custom message handler from the specified content world in your JavaScript code.

func removeAllScriptMessageHandlers(from: WKContentWorld)

Uninstalls all custom message handlers from the specified content world in your JavaScript code.

func removeAllScriptMessageHandlers()

Uninstalls all custom message handlers associated with the user content controller.

protocol WKScriptMessageHandler

An interface for receiving messages from JavaScript code running in a webpage.

protocol WKScriptMessageHandlerWithReply

An interface for responding to messages from JavaScript code running in a webpage.

