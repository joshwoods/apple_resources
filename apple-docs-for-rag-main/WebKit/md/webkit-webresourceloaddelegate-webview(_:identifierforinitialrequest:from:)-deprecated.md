

- WebKit
- WebResourceLoadDelegate
-  webView(\_:identifierForInitialRequest:from:) Deprecated

Instance Method

# webView(\_:identifierForInitialRequest:from:)

Returns an identifier object used to track the progress of loading a single resource.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    identifierForInitialRequest request: URLRequest!,
    from dataSource: WebDataSource!
) -> Any!
```

## Parameters 

`sender`  

The web view that sent this message.

`request`  

The request that initiated this load for `dataSource`.

`dataSource`  

The data source for this web view.

## Return Value

An identifier object that is retained by `sender` and passed as a parameter to all other delegate messages pertaining to this resource.

## Discussion

Delegates might implement this method to begin tracking the progress of loading an individual resource. Note that this method is invoked once per load where as the webView(_:resource:willSend:redirectResponse:from:) method may be invoked multiple times.

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

