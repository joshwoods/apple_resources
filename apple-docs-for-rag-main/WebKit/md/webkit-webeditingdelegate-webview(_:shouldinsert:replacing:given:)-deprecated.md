

- WebKit
- WebEditingDelegate
-  webView(\_:shouldInsert:replacing:given:) Deprecated

Instance Method

# webView(\_:shouldInsert:replacing:given:)

Returns whether the user should be allowed to insert a node in place of a range of content.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    shouldInsert node: DOMNode!,
    replacing range: DOMRange!,
    given action: WebViewInsertAction
) -> Bool
```

## Parameters 

`webView`  

The web view that the user is editing.

`node`  

The content to insert.

`range`  

The portion of the content that is replaced with `node`.

`action`  

Indicates the type of user action that initiated the insertion.

## Return Value

true if the user should be allowed to insert `node` in `webView`; otherwise, false.

## Discussion

This method may perform an alternate action—for example, insert a different node—and return false.

## See Also

### Related Documentation

func webViewDidChange(Notification!)

Sent by the default notification center when the user changes content in the web view.

Deprecated

func webView(WebView!, shouldInsertText: String!, replacing: DOMRange!, given: WebViewInsertAction) -> Bool

Returns whether a user should be allowed to insert text in place of a range of content.

Deprecated

