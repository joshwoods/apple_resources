

- WebKit
- WebDocumentRepresentation
-  finishedLoading(with:) Deprecated

Instance Method

# finishedLoading(with:)

Invoked when a data source finishes loading its content.

macOS 10.3–10.14Deprecated

``` source
func finishedLoading(with dataSource: WebDataSource!)
```

**Required**

## Parameters 

`dataSource`  

A `WebDataSource` object that identifies the request that finished loading.

## See Also

### Related Documentation

func setDataSource(WebDataSource!)

Sets the receiver’s data source.

**Required**

Deprecated

### Loading content

func receivedData(Data!, with: WebDataSource!)

Invoked when a data source has received some data.

**Required**

Deprecated

func receivedError((any Error)!, with: WebDataSource!)

Invoked when a data source receives an error loading its content.

**Required**

Deprecated

