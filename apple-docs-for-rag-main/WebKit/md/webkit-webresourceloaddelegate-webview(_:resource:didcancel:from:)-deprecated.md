

- WebKit
- WebResourceLoadDelegate
-  webView(\_:resource:didCancel:from:) Deprecated

Instance Method

# webView(\_:resource:didCancel:from:)

Invoked when an authentication challenge for a resource was canceled.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    resource identifier: Any!,
    didCancel challenge: URLAuthenticationChallenge!,
    from dataSource: WebDataSource!
)
```

## Parameters 

`sender`  

The web view that sent this message.

`identifier`  

An identifier object used to track the resource being loaded by `dataSource`.

`challenge`  

The authentication challenge that was canceled.

`dataSource`  

The data source for this web view.

## See Also

### Authenticating Resources

func webView(WebView!, resource: Any!, didReceive: URLAuthenticationChallenge!, from: WebDataSource!)

Invoked when an authentication challenge has been received for a resource.

Deprecated

