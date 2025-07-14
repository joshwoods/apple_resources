

- WebKit
- WebResourceLoadDelegate
-  webView(\_:plugInFailedWithError:dataSource:) Deprecated

Instance Method

# webView(\_:plugInFailedWithError:dataSource:)

Invoked when a plug-in fails to load.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    plugInFailedWithError error: (any Error)!,
    dataSource: WebDataSource!
)
```

## Parameters 

`sender`  

The web view that sent this message.

`error`  

The error that occurred during the process of loading that resource.

The `userInfo` dictionary of `error` may contain additional information about the failure. If the `userInfo` dictionary is not `nil`, it may contain some or all of these key-value pairs. The value of the `NSErrorFailingURLKey` key is a URL string of the `SRC` attribute. The value of the WebKitErrorPlugInNameKey key is a string containing the plug-in’s name. The value for the WebKitErrorPlugInPageURLStringKey key is a URL string of the `PLUGINSPAGE` attribute. The value of the WebKitErrorMIMETypeKey key is a string of the `TYPE` attribute.

`dataSource`  

The data source for this web view.

## Discussion

This method might be invoked if a plug-in is not found, fails to load, or is not available for some reason. Delegates might implement this method to display or log a detailed error message. If you do not implement this method, no action is taken.

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

func webView(WebView!, resource: Any!, didReceiveContentLength: Int, from: WebDataSource!)

Invoked when some of the data for a given resource has arrived.

Deprecated

func webView(WebView!, resource: Any!, didFailLoadingWithError: (any Error)!, from: WebDataSource!)

Invoked when a resource failed to load.

Deprecated

