

- WebKit
-  WebEditingDelegate Deprecated

Protocol

# WebEditingDelegate

macOS 10.3–10.14Deprecated

``` source
protocol WebEditingDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func undoManager(for: WebView!) -> UndoManager!

Returns the undo manager to be used by a web view.

func webView(WebView!, doCommandBy: Selector!) -> Bool

Returns whether the receiver performs a command instead of the web view.

func webView(WebView!, shouldApplyStyle: DOMCSSStyleDeclaration!, toElementsIn: DOMRange!) -> Bool

Returns whether the user should be allowed to apply a style to a range of content.

func webView(WebView!, shouldBeginEditingIn: DOMRange!) -> Bool

Returns whether the user is allowed to edit a range of content in a web view.

func webView(WebView!, shouldChangeSelectedDOMRange: DOMRange!, to: DOMRange!, affinity: NSSelectionAffinity, stillSelecting: Bool) -> Bool

Returns whether the user should be allowed to change the selected range.

func webView(WebView!, shouldChangeTypingStyle: DOMCSSStyleDeclaration!, toStyle: DOMCSSStyleDeclaration!) -> Bool

Returns whether the user should be allowed to change the typing style in a web view.

func webView(WebView!, shouldDelete: DOMRange!) -> Bool

Returns whether the user should be allowed to delete a range of content.

func webView(WebView!, shouldEndEditingIn: DOMRange!) -> Bool

Returns whether the user should be allowed to end editing.

func webView(WebView!, shouldInsert: DOMNode!, replacing: DOMRange!, given: WebViewInsertAction) -> Bool

Returns whether the user should be allowed to insert a node in place of a range of content.

func webView(WebView!, shouldInsertText: String!, replacing: DOMRange!, given: WebViewInsertAction) -> Bool

Returns whether a user should be allowed to insert text in place of a range of content.

func webViewDidBeginEditing(Notification!)

Sent by the default notification center when the user begins editing the web view.

func webViewDidChange(Notification!)

Sent by the default notification center when the user changes content in the web view.

func webViewDidChangeSelection(Notification!)

Sent by the default notification center when the user changes the selection in the web view.

func webViewDidChangeTypingStyle(Notification!)

Sent by the default notification center when the user changes the typing style in the web view.

func webViewDidEndEditing(Notification!)

Sent by the default notification center when the user stops editing the web view.

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

protocol WebUIDelegate

Web view user interface delegates implement this protocol to control the opening of new windows, augment the behavior of default menu items displayed when the user clicks elements, and perform other user interface–related tasks. These methods can be invoked as a result of handling JavaScript or other plug-in content. Delegates that display more than one web view per window, for example, need to implement some of these methods to handle that case. The default implementation assumes one window per web view, so non-conventional user interfaces might implement a user interface delegate.

Deprecated

