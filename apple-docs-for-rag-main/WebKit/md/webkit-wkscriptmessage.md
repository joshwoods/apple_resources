

- WebKit
-  WKScriptMessage 

Class

# WKScriptMessage

An object that encapsulates a message sent by JavaScript code from a webpage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
class WKScriptMessage
```

## Overview

Use a WKScriptMessage object to get details about a JavaScript message sent to a custom message handler in your app. You don’t create WKScriptMessage objects directly. When JavaScript code targets one of your app’s message handlers, the WKUserContentController object of the web view creates a WKScriptMessage object and delivers it to the message handler’s delegate method. Use the object you’re provided to process the message and provide an appropriate response.

For more information about handling script messages, see the WKScriptMessageHandler and WKScriptMessageHandlerWithReply protocols. For information about how to register message handlers, see the methods of WKUserContentController.

## Topics

### Getting the Message Contents

var body: Any

The body of the message.

### Getting Message-Related Information

var frameInfo: WKFrameInfo

The frame that sent the message.

var webView: WKWebView?

The web view that sent the message.

var world: WKContentWorld

The namespace in which the JavaScript code executes.

### Getting the Message Handler’s Name

var name: String

The name of the message handler to which the message is sent.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Receiving Messages

func userContentController(WKUserContentController, didReceive: WKScriptMessage)

Tells the handler that a webpage sent a script message.

**Required**

