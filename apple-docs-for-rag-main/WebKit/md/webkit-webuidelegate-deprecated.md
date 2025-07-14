

- WebKit
-  WebUIDelegate Deprecated

Protocol

# WebUIDelegate

Web view user interface delegates implement this protocol to control the opening of new windows, augment the behavior of default menu items displayed when the user clicks elements, and perform other user interface–related tasks. These methods can be invoked as a result of handling JavaScript or other plug-in content. Delegates that display more than one web view per window, for example, need to implement some of these methods to handle that case. The default implementation assumes one window per web view, so non-conventional user interfaces might implement a user interface delegate.

macOS 10.3–10.14Deprecated

``` source
protocol WebUIDelegate : NSObjectProtocol
```

## Topics

### Creating and Closing Windows

func webView(WebView!, createWebViewModalDialogWith: URLRequest!) -> WebView!

Creates a modal window containing a web view that loads the specified request.

func webViewRunModal(WebView!)

Displays a web view in a modal window.

func webView(WebView!, createWebViewWith: URLRequest!) -> WebView!

Creates a window containing a web view to load the specified request.

func webViewClose(WebView!)

Closes a web view in a window.

### Moving and Resizing Windows

func webViewIsResizable(WebView!) -> Bool

Returns a Boolean value indicating whether a web view’s window can be resized.

func webView(WebView!, setResizable: Bool)

Sets whether a web view’s window can be resized.

func webView(WebView!, setFrame: NSRect)

Sets the frame rectangle of a web view’s window to the specified frame size.

func webViewFrame(WebView!) -> NSRect

Returns the frame rectangle of a web view’s window.

### Making Windows Key and Main

func webViewFocus(WebView!)

Brings a web view’s window to the front and makes it the active window.

func webViewUnfocus(WebView!)

Relinquishes focus on a web view’s window.

### Ordering Windows

func webViewShow(WebView!)

Displays a web view’s window and moves it to the front.

### Working with the Responder Chain

func webViewFirstResponder(WebView!) -> NSResponder!

Returns the first responder of the web view’s window.

func webView(WebView!, makeFirstResponder: NSResponder!)

Sets the first responder of a web view’s window to the specified view.

### Handling Mouse Events

func webView(WebView!, mouseDidMoveOverElement: [AnyHashable : Any]!, modifierFlags: Int)

Updates information about the element the user is mousing over.

func webView(WebView!, contextMenuItemsForElement: [AnyHashable : Any]!, defaultMenuItems: [Any]!) -> [Any]!

Returns menu items to display in an element’s contextual menu.

### Opening Panels

func webView(WebView!, runJavaScriptAlertPanelWithMessage: String!, initiatedBy: WebFrame!)

Displays a JavaScript alert panel containing the specified message.

func webView(WebView!, runJavaScriptConfirmPanelWithMessage: String!, initiatedBy: WebFrame!) -> Bool

Displays a JavaScript confirmation panel with the specified message.

func webView(WebView!, runJavaScriptTextInputPanelWithPrompt: String!, defaultText: String!, initiatedBy: WebFrame!) -> String!

Displays a JavaScript text input panel and returns the entered text.

func webView(WebView!, runOpenPanelForFileButtonWith: (any WebOpenPanelResultListener)!)

Displays an open panel for a file input control.

func webView(WebView!, runOpenPanelForFileButtonWith: (any WebOpenPanelResultListener)!, allowMultipleFiles: Bool)

Displays an open panel for a file input control.

func webView(WebView!, runBeforeUnloadConfirmPanelWithMessage: String!, initiatedBy: WebFrame!) -> Bool

Displays a confirmation panel containing the specified message before a window closes.

### Displaying Status Messages

func webView(WebView!, setStatusText: String!)

Sets the status message displayed by a web view’s window, if any, to the specified text.

func webViewStatusText(WebView!) -> String!

Returns the current status message from a web view’s window.

### Managing Toolbars and the Status Bar

func webViewAreToolbarsVisible(WebView!) -> Bool

Returns a Boolean value indicating whether any toolbars are visible in a web view’s window.

func webView(WebView!, setToolbarsVisible: Bool)

Sets whether a web view’s toolbars should be visible.

func webViewIsStatusBarVisible(WebView!) -> Bool

Returns a Boolean value indicating whether the status bar in a web view’s window is visible.

func webView(WebView!, setStatusBarVisible: Bool)

Sets the visibility of the status bar in a web view’s window.

### Controlling Drag Behavior

func webView(WebView!, dragDestinationActionMaskFor: (any NSDraggingInfo)!) -> Int

Returns a mask indicating which drag operations are allowed by the sender.

func webView(WebView!, dragSourceActionMaskFor: NSPoint) -> Int

Returns a mask indicating which drag-source actions are allowed for a drag that begins at the specified location.

func webView(WebView!, willPerform: WebDragDestinationAction, for: (any NSDraggingInfo)!)

Tells the receiver that the sending web view will perform the specified drag-destination action.

func webView(WebView!, willPerform: WebDragSourceAction, from: NSPoint, with: NSPasteboard!)

Tells the receiver that the sending web view will perform the specified drag-source action.

### Controlling Other Behaviors

func webView(WebView!, shouldPerformAction: Selector!, fromSender: Any!) -> Bool

Returns a Boolean value that indicates whether the action sent by the specified object should be performed.

func webView(WebView!, validate: (any NSValidatedUserInterfaceItem)!, defaultValidation: Bool) -> Bool

Returns a Boolean value that indicates whether the specified user interface item is valid.

### Printing

func webView(WebView!, print: WebFrameView!)

Prints the contents of a web frame view.

func webViewHeaderHeight(WebView!) -> Float

Returns the height of the web view’s printed page header.

func webViewFooterHeight(WebView!) -> Float

Returns the height of the web view’s printed page footer.

func webView(WebView!, drawHeaderIn: NSRect)

Draws the web view’s header in the specified rectangle.

func webView(WebView!, drawFooterIn: NSRect)

Draws the web view’s footer in the specified rectangle.

### Constants

Menu Item Tags

Tags that define the types of default menu items passed to the webView(_:contextMenuItemsForElement:defaultMenuItems:) method.

struct WebDragDestinationAction

Actions that the destination object of a drag operation can perform.

struct WebDragSourceAction

Actions that the source object of a drag operation can perform.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting Up a Web View (Legacy)

class WebView

`WebView` is the core view class in the WebKit framework that manages interactions between the `WebFrame` and `WebFrameView` classes. To embed web content in your application, you just create a `WebView` object, attach it to a window, and send a load(_:) message to its main frame.

Deprecated

class WebPreferences

WebPreferences encapsulates the preferences you can change per WebView object. These preferences include font, text encoding, and image settings. Normally a WebView object uses the standard preferences returned by the standard() class method. However, you can modify the preferences for individual WebView instances too. Use the preferencesIdentifier WebView method to change a WebView object’s preferences, or to share preferences between WebView objects. Use the autosaves method to specify if the preferences object should be automatically saved to the user defaults database.

Deprecated

protocol WebEditingDelegateDeprecated

