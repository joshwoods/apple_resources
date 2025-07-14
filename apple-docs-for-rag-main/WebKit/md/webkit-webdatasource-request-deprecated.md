

- WebKit
- WebDataSource
-  request Deprecated

Instance Property

# request

The request that was used to create the data source.

macOS 10.3–10.14Deprecated

``` source
var request: NSMutableURLRequest! { get }
```

## Discussion

This URL may be different from the original request from initialRequest.

A web view’s resource load delegate may modify requests by implementing the webView:resource:willSendRequest:redirectResponse:fromDataSource: method.

## See Also

### Getting the request and response

var initialRequest: URLRequest!

A reference to the original request that was used to load the web content.

Deprecated

var response: URLResponse!

The response for this data source.

Deprecated

