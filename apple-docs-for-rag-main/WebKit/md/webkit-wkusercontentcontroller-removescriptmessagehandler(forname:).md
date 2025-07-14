

- WebKit
- WKUserContentController
-  removeScriptMessageHandler(forName:) 

Instance Method

# removeScriptMessageHandler(forName:)

Uninstalls the custom message handler with the specified name from your JavaScript code.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
func removeScriptMessageHandler(forName name: String)
```

## Parameters 

`name`  

The name of the message handler to remove. If no message handler with this name exists in the user content controller, this method does nothing.

## Discussion

Use this method to remove a message handler that you previously installed using the add(_:name:) method. This method removes the message handler from the page content world — that is, the content world available from the page property of WKContentWorld. If you installed the message handler in a different content world, this method doesn’t remove it.

## See Also

### Adding and Removing Message Handlers

func add(any WKScriptMessageHandler, name: String)

Installs a message handler that you can call from your JavaScript code.

func add(any WKScriptMessageHandler, contentWorld: WKContentWorld, name: String)

Installs a message handler that you can call from the specified content world in your JavaScript code.

func addScriptMessageHandler(any WKScriptMessageHandlerWithReply, contentWorld: WKContentWorld, name: String)

Installs a message handler that returns a reply to your JavaScript code.

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

