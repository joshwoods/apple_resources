

- WebKit
- WebEditingDelegate
-  webView(\_:shouldChangeTypingStyle:toStyle:) Deprecated

Instance Method

# webView(\_:shouldChangeTypingStyle:toStyle:)

Returns whether the user should be allowed to change the typing style in a web view.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    shouldChangeTypingStyle currentStyle: DOMCSSStyleDeclaration!,
    toStyle proposedStyle: DOMCSSStyleDeclaration!
) -> Bool
```

## Parameters 

`webView`  

The web view that the user is editing.

`currentStyle`  

The old style the user wants to change.

`proposedStyle`  

The new style the user wants to set.

## Return Value

true if the user should be allowed to change the typing style in `webView` to `proposedStyle`; otherwise, false.

## Discussion

You can implement this method to take some other action—for example, set the typing style to a different style—and return false .

## See Also

### Related Documentation

func webViewDidChangeTypingStyle(Notification!)

Sent by the default notification center when the user changes the typing style in the web view.

Deprecated

