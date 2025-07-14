

- WebKit
- WebResourceLoadDelegate
-  webView(\_:resource:didReceiveContentLength:from:) Deprecated

Instance Method

# webView(\_:resource:didReceiveContentLength:from:)

Invoked when some of the data for a given resource has arrived.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    resource identifier: Any!,
    didReceiveContentLength length: Int,
    from dataSource: WebDataSource!
)
```

## Parameters 

`sender`  

The web view that sent this message.

`identifier`  

An identifier object used to track the resource being loaded by `dataSource`.

`length`  

The amount of incremental data received for this resource—the amount of data loaded since the last time this method was invoked for this resource, not the total amount received for this resource.

The `length` parameter type was changed from type `unsigned int` to type `NSUInteger` in OS X v10.5.

`dataSource`  

The data source for this web view.

## Discussion

Delegates might implement this method to update the load status of an individual resource.

## See Also

### Loading Content

func webView(WebView!, resource: Any!, willSend: URLRequest!, redirectResponse: URLResponse!, from: WebDataSource!) -> URLRequest!

Invoked before a request is initiated for a resource and returns a possibly modified request.

Deprecated

func webView(WebView!, resource: Any!, didFinishLoadingFrom: WebDataSource!)

Invoked when all of the data for a given resource is loaded.

Deprecated

func webView(WebView!, resource: Any!, didReceive: URLResponse!, from: WebDataSource!)

Invoked after a resource has been loaded.

Deprecated

func webView(WebView!, resource: Any!, didFailLoadingWithError: (any Error)!, from: WebDataSource!)

Invoked when a resource failed to load.

Deprecated

func webView(WebView!, plugInFailedWithError: (any Error)!, dataSource: WebDataSource!)

Invoked when a plug-in fails to load.

Deprecated

