

- WebKit
- WebResourceLoadDelegate
-  webView(\_:resource:willSend:redirectResponse:from:) Deprecated

Instance Method

# webView(\_:resource:willSend:redirectResponse:from:)

Invoked before a request is initiated for a resource and returns a possibly modified request.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    resource identifier: Any!,
    willSend request: URLRequest!,
    redirectResponse: URLResponse!,
    from dataSource: WebDataSource!
) -> URLRequest!
```

## Parameters 

`sender`  

The web view that sent this message.

`identifier`  

An identifier object used to track the resource being loaded by `dataSource`.

`request`  

The request that is sent.

`redirectResponse`  

The redirect server response. If `nil`, there is no redirect in progress.

`dataSource`  

The data source for this web view.

## Return Value

A possibly modified request.

## Discussion

Delegates might implement this method to modify resource requests before they are sent. Note that this method might be invoked multiple times per load (as a result of a server redirect) where as the webView(_:identifierForInitialRequest:from:) method is invoked once.

## See Also

### Loading Content

func webView(WebView!, resource: Any!, didFinishLoadingFrom: WebDataSource!)

Invoked when all of the data for a given resource is loaded.

Deprecated

func webView(WebView!, resource: Any!, didReceive: URLResponse!, from: WebDataSource!)

Invoked after a resource has been loaded.

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

