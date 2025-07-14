

- WebKit
- WebEditingDelegate
-  webView(\_:shouldInsertText:replacing:given:) Deprecated

Instance Method

# webView(\_:shouldInsertText:replacing:given:)

Returns whether a user should be allowed to insert text in place of a range of content.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    shouldInsertText text: String!,
    replacing range: DOMRange!,
    given action: WebViewInsertAction
) -> Bool
```

## Parameters 

`webView`  

The web view that the user is editing.

`text`  

The text to insert.

`range`  

The portion of the document that will be replaced with `text`.

`action`  

Indicates the type of user action that initiated the insertion.

## Return Value

true if the user should be allowed to insert `text` in `webView`; otherwise, false.

## Discussion

This method may perform an alternate action—for example, insert different text—and return false.

## See Also

### Related Documentation

func webViewDidChange(Notification!)

Sent by the default notification center when the user changes content in the web view.

Deprecated

func webView(WebView!, shouldInsert: DOMNode!, replacing: DOMRange!, given: WebViewInsertAction) -> Bool

Returns whether the user should be allowed to insert a node in place of a range of content.

Deprecated

