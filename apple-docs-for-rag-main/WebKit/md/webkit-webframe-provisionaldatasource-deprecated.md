

- WebKit
- WebFrame
-  provisionalDataSource Deprecated

Instance Property

# provisionalDataSource

The provisional data source, or `nil` if either a load request is not in progress or a load request has completed.

macOS 10.3–10.14Deprecated

``` source
var provisionalDataSource: WebDataSource! { get }
```

## Discussion

Use the load(_:) method to initiate an asynchronous client request, which creates a provisional data source. The provisional data source transitions to a committed data source once any data is received.

## See Also

### Getting the Data Source

var dataSource: WebDataSource?

The committed data source.

Deprecated

