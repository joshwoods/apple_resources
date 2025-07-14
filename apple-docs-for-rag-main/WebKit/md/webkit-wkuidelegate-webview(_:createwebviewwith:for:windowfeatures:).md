

- WebKit
- WKUIDelegate
-  webView(\_:createWebViewWith:for:windowFeatures:) 

Instance Method

# webView(\_:createWebViewWith:for:windowFeatures:)

Creates a new web view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    createWebViewWith configuration: WKWebViewConfiguration,
    for navigationAction: WKNavigationAction,
    windowFeatures: WKWindowFeatures
) -> WKWebView?
```

## Parameters 

`webView`  

The web view invoking the delegate method.

`configuration`  

The configuration to use when creating the new web view.

`navigationAction`  

The navigation action causing the new web view to be created.

`windowFeatures`  

Window features requested by the webpage.

## Return Value

A new web view or `nil`.

## Discussion

The web view returned must be created with the specified configuration. WebKit loads the request in the returned web view.

## See Also

### Creating and closing the web view

func webViewDidClose(WKWebView)

Notifies your app that the DOM window closed successfully.

