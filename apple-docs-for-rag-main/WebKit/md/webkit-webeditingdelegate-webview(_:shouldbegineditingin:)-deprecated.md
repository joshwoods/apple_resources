

- WebKit
- WebEditingDelegate
-  webView(\_:shouldBeginEditingIn:) Deprecated

Instance Method

# webView(\_:shouldBeginEditingIn:)

Returns whether the user is allowed to edit a range of content in a web view.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    shouldBeginEditingIn range: DOMRange!
) -> Bool
```

## Parameters 

`webView`  

The web view that the user is editing.

`range`  

The section of the begin-editing request; used to determine if editing is allowed. Typically, `range` is not the current selection but may becomes the current selection if this method returns true.

## Return Value

true if the user is allowed to edit `webView`; otherwise, false.

## Discussion

This method is invoked when a web view attempts to become the first responder or when the user drops an object on it.

## See Also

### Related Documentation

func webView(WebView!, shouldEndEditingIn: DOMRange!) -> Bool

Returns whether the user should be allowed to end editing.

Deprecated

func webViewDidBeginEditing(Notification!)

Sent by the default notification center when the user begins editing the web view.

Deprecated

