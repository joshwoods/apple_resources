

- WebKit
- WebDataSource
-  subresources Deprecated

Instance Property

# subresources

The data source’s subresources that have finished downloading.

macOS 10.3–10.14Deprecated

``` source
var subresources: [Any]! { get }
```

## See Also

### Accessing subresources

var mainResource: WebResource!

A`WebResource` object representing the data source.

Deprecated

func addSubresource(WebResource!)

Adds a resource to the data source’s list of subresources.

Deprecated

func subresource(for: URL!) -> WebResource!

Returns a subresource for the given URL.

Deprecated

