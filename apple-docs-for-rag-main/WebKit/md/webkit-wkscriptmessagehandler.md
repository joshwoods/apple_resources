

- WebKit
-  WKScriptMessageHandler 

Protocol

# WKScriptMessageHandler

An interface for receiving messages from JavaScript code running in a webpage.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
@MainActor
protocol WKScriptMessageHandler : NSObjectProtocol
```

## Overview

Adopt the WKScriptMessageHandler protocol when your app needs a way to respond to JavaScript messages in the web view. When JavaScript code sends a message that specifically targets your message handler, WebKit calls your handler’s userContentController(_:didReceive:) method. Use that method to implement your response. For example, you might update other parts of your app in response to web content changes.

To call your message handler from JavaScript, call the function `window.webkit.messageHandlers.``.postMessage(``)` in your code. You specify the value of when you install your message handler in a WKUserContentController object.

Note

If you want to provide a response back to JavaScript, implement your message handler using the WKScriptMessageHandlerWithReply protocol instead.

## Topics

### Receiving Messages

func userContentController(WKUserContentController, didReceive: WKScriptMessage)

Tells the handler that a webpage sent a script message.

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

protocol WKScriptMessageHandlerWithReply

An interface for responding to messages from JavaScript code running in a webpage.

