

- WebKit
- WebResourceLoadDelegate
-  webView(\_:resource:didReceive:from:) Deprecated

Instance Method

# webView(\_:resource:didReceive:from:)

Invoked after a resource has been loaded.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    resource identifier: Any!,
    didReceive response: URLResponse!,
    from dataSource: WebDataSource!
)
```

## Parameters 

`sender`  

The web view that sent this message.

`identifier`  

An identifier object used to track the resource being loaded by `dataSource`.

`response`  

The reply that was received.

`dataSource`  

The data source for this web view.

## Discussion

In some rare cases, multiple responses may be received for a single resource. This happens in the case of multipart/x-mixed-replace, also known as a *server push*. In this case, delegates should assume that the progress of loading this resource restarts, and the expected content length may change.

## See Also

### Loading Content

func webView(WebView!, resource: Any!, willSend: URLRequest!, redirectResponse: URLResponse!, from: WebDataSource!) -> URLRequest!

Invoked before a request is initiated for a resource and returns a possibly modified request.

Deprecated

func webView(WebView!, resource: Any!, didFinishLoadingFrom: WebDataSource!)

Invoked when all of the data for a given resource is loaded.

Deprecated

func webView(WebView!, resource: Any!, didReceiveContentLength: Int, from: WebDataSource!)

Invoked when some of the data for a given resource has arrived.

Deprecated

func webView(WebView!, resource: Any!, didFailLoadingWithError: (any Error)!, from: WebDataSource!)

Invoked when a resource failed to load.

Deprecated

func webView(WebView!, plugInFailedWithError: (any Error)!, dataSource: WebDataSource!)

Invoked when a plug-in fails to load.

Deprecated

