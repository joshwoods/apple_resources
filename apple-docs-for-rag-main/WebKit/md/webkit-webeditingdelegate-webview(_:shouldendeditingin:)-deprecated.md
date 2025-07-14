

- WebKit
- WebEditingDelegate
-  webView(\_:shouldEndEditingIn:) Deprecated

Instance Method

# webView(\_:shouldEndEditingIn:)

Returns whether the user should be allowed to end editing.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    shouldEndEditingIn range: DOMRange!
) -> Bool
```

## Parameters 

`webView`  

The web view that the user is editing.

`range`  

Typically, the current selection, although it might not be. Use the `range` parameter to help determine whether the user can end editing.

## Return Value

true if the user should be allowed to end editing `webView`; otherwise, false. If this method returnstrue, `webView` ends editing and resigns as the first responder.

## Discussion

This method is invoked when a web view attempts to resign as the first responder.

## See Also

### Related Documentation

func webView(WebView!, shouldBeginEditingIn: DOMRange!) -> Bool

Returns whether the user is allowed to edit a range of content in a web view.

Deprecated

func webViewDidEndEditing(Notification!)

Sent by the default notification center when the user stops editing the web view.

Deprecated

