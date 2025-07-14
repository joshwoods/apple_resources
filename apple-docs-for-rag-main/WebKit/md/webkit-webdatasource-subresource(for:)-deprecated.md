

- WebKit
- WebDataSource
-  subresource(for:) Deprecated

Instance Method

# subresource(for:)

Returns a subresource for the given URL.

macOS 10.3–10.14Deprecated

``` source
func subresource(for URL: URL!) -> WebResource!
```

## Parameters 

`URL`  

The subresource’s URL.

## Return Value

The subresource for `URL` or `nil` if the data source hasn’t finished downloading the subresource.

## See Also

### Accessing subresources

var mainResource: WebResource!

A`WebResource` object representing the data source.

Deprecated

func addSubresource(WebResource!)

Adds a resource to the data source’s list of subresources.

Deprecated

var subresources: [Any]!

The data source’s subresources that have finished downloading.

Deprecated

