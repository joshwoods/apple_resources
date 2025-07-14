

- WebKit
- WebResourceLoadDelegate
-  webView(\_:resource:didReceive:from:) Deprecated

Instance Method

# webView(\_:resource:didReceive:from:)

Invoked when an authentication challenge has been received for a resource.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    resource identifier: Any!,
    didReceive challenge: URLAuthenticationChallenge!,
    from dataSource: WebDataSource!
)
```

## Parameters 

`sender`  

The web view that sent this message.

`identifier`  

An identifier object used to track the resource being loaded by `dataSource`.

`challenge`  

The authentication challenge that was received.

`dataSource`  

The data source for this web view.

## See Also

### Authenticating Resources

func webView(WebView!, resource: Any!, didCancel: URLAuthenticationChallenge!, from: WebDataSource!)

Invoked when an authentication challenge for a resource was canceled.

Deprecated

