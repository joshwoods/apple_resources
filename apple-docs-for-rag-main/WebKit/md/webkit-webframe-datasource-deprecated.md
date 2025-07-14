

- WebKit
- WebFrame
-  dataSource Deprecated

Instance Property

# dataSource

The committed data source.

macOS 10.3–10.14Deprecated

``` source
var dataSource: WebDataSource? { get }
```

## Discussion

`nil` if the provisional data source is not done loading.

## See Also

### Getting the Data Source

var provisionalDataSource: WebDataSource!

The provisional data source, or `nil` if either a load request is not in progress or a load request has completed.

Deprecated

