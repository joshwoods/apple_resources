

- WebKit
- WebEditingDelegate
-  webView(\_:shouldDelete:) Deprecated

Instance Method

# webView(\_:shouldDelete:)

Returns whether the user should be allowed to delete a range of content.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    shouldDelete range: DOMRange!
) -> Bool
```

## Parameters 

`webView`  

The web view that the user is editing.

`range`  

The range of the content to delete.

## Return Value

true if the user should be allowed to delete the content specified by `range`; otherwise, false.

## Discussion

This method may perform an alternate action—for example, delete a different range—and return false.

## See Also

### Related Documentation

func webViewDidChange(Notification!)

Sent by the default notification center when the user changes content in the web view.

Deprecated

