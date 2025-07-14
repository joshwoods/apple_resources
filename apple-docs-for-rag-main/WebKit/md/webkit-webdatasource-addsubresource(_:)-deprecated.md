

- WebKit
- WebDataSource
-  addSubresource(\_:) Deprecated

Instance Method

# addSubresource(\_:)

Adds a resource to the data source’s list of subresources.

macOS 10.3–10.14Deprecated

``` source
func addSubresource(_ subresource: WebResource!)
```

## Parameters 

`subresource`  

The resource to add to the data source.

## Discussion

If the data source needs to reload the resource’s URL, it loads the data from `subresource` instead of the network. For example, use this method if you want to use a previously downloaded image rather than accessing the network to reload a resource. If the data source already has a resource with the same URL as `subresource`, then this method replaces it.

## See Also

### Accessing subresources

var mainResource: WebResource!

A`WebResource` object representing the data source.

Deprecated

func subresource(for: URL!) -> WebResource!

Returns a subresource for the given URL.

Deprecated

var subresources: [Any]!

The data source’s subresources that have finished downloading.

Deprecated

