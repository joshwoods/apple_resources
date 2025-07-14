

- WebKit
- WebUIDelegate
-  webView(\_:mouseDidMoveOverElement:modifierFlags:) Deprecated

Instance Method

# webView(\_:mouseDidMoveOverElement:modifierFlags:)

Updates information about the element the user is mousing over.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    mouseDidMoveOverElement elementInformation: [AnyHashable : Any]!,
    modifierFlags: Int
)
```

## Parameters 

`sender`  

The web view that sent the message.

`elementInformation`  

A dictionary that describes the element under the mouse, or `nil`. See “Constants” in WebView for information about the key-value pairs in this dictionary.

`modifierFlags`  

An integer bit field that indicates the modifier keys in effect during the event. See “Modifier Flags” in NSEvent for information about possible modifiers. Note that this parameter was changed from an `unsigned int` to an `NSUInteger` in OS X v10.5.

## See Also

### Handling Mouse Events

func webView(WebView!, contextMenuItemsForElement: [AnyHashable : Any]!, defaultMenuItems: [Any]!) -> [Any]!

Returns menu items to display in an element’s contextual menu.

Deprecated

