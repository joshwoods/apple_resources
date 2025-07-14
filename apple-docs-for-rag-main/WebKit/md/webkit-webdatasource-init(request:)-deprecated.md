

- WebKit
- WebDataSource
-  init(request:) Deprecated

Initializer

# init(request:)

initializes a data source with a URL request.

macOS 10.3–10.14Deprecated

``` source
init!(request: URLRequest!)
```

## Parameters 

`request`  

The URL request used to load the web content.

## Return Value

The initialized web data source.

## Discussion

This method is the designated initializer for `WebDataSource` objects. Normally, `WebFrame` objects create their data sources, so you should not invoke this method directly.

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

