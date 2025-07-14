

- WebKit
- WebDataSource
-  mainResource Deprecated

Instance Property

# mainResource

A`WebResource` object representing the data source.

macOS 10.3–10.14Deprecated

``` source
var mainResource: WebResource! { get }
```

## See Also

### Accessing subresources

func addSubresource(WebResource!)

Adds a resource to the data source’s list of subresources.

Deprecated

func subresource(for: URL!) -> WebResource!

Returns a subresource for the given URL.

Deprecated

var subresources: [Any]!

The data source’s subresources that have finished downloading.

Deprecated

