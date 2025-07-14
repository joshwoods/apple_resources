

- WebKit
- WebDataSource
-  webArchive Deprecated

Instance Property

# webArchive

A web archive representing the data source, its subresources, and subframes.

macOS 10.3–10.14Deprecated

``` source
var webArchive: WebArchive! { get }
```

## Discussion

In the case of HTML, if the current content is preferred, then send webArchive to the appropriate DOM object.

## See Also

### Related Documentation

var mainResource: WebResource!

A`WebResource` object representing the data source.

Deprecated

