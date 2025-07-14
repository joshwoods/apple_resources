

- WebKit
- WKUserContentController
-  removeAllScriptMessageHandlers() 

Instance Method

# removeAllScriptMessageHandlers()

Uninstalls all custom message handlers associated with the user content controller.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
func removeAllScriptMessageHandlers()
```

## Discussion

Use this method to remove all message handlers in all content worlds in your JavaScript code.

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

protocol WKScriptMessageHandler

An interface for receiving messages from JavaScript code running in a webpage.

protocol WKScriptMessageHandlerWithReply

An interface for responding to messages from JavaScript code running in a webpage.

