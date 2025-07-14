

- WebKit
-  WKScriptMessageHandlerWithReply 

Protocol

# WKScriptMessageHandlerWithReply

An interface for responding to messages from JavaScript code running in a webpage.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
@MainActor
protocol WKScriptMessageHandlerWithReply : NSObjectProtocol
```

## Overview

Adopt the WKScriptMessageHandlerWithReply protocol when your app needs to receive JavaScript messages from a web view and provide an appropriate response. When JavaScript code sends a message that specifically targets your message handler, WebKit calls your handler’s userContentController(_:didReceive:replyHandler:) method. Use that method to process the message and provide your response.

To call your message handler from JavaScript, send a message to `window.webkit.messageHandlers.``.postMessage(``)` in your code. You specify the name of your message handler when you add it to a WKUserContentController object.

Note

If you don’t need to provide a response back to JavaScript, implement your message handler using the WKScriptMessageHandler protocol instead.

## Topics

### Receiving Messages

func userContentController(WKUserContentController, didReceive: WKScriptMessage, replyHandler: (Any?, String?) -> Void)

Tells the handler that a webpage sent a script message that included a reply.

**Required**

class WKScriptMessage

An object that encapsulates a message sent by JavaScript code from a webpage.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Adding and Removing Message Handlers

func add(any WKScriptMessageHandler, name: String)

Installs a message handler that you can call from your JavaScript code.

func add(any WKScriptMessageHandler, contentWorld: WKContentWorld, name: String)

Installs a message handler that you can call from the specified content world in your JavaScript code.

func addScriptMessageHandler(any WKScriptMessageHandlerWithReply, contentWorld: WKContentWorld, name: String)

Installs a message handler that returns a reply to your JavaScript code.

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

