

- WebKit
- WebDocumentRepresentation
-  receivedData(\_:with:) Deprecated

Instance Method

# receivedData(\_:with:)

Invoked when a data source has received some data.

macOS 10.3–10.14Deprecated

``` source
func receivedData(
    _ data: Data!,
    with dataSource: WebDataSource!
)
```

**Required**

## Parameters 

`data`  

An `NSData` object containing the data received.

`dataSource`  

A `WebDataSource` object that identifies the request that generated this data.

## Discussion

Data is loaded incrementally, so this method may be invoked multiple times. The receiver is responsible for accumulating this data.

## See Also

### Loading content

func receivedError((any Error)!, with: WebDataSource!)

Invoked when a data source receives an error loading its content.

**Required**

Deprecated

func finishedLoading(with: WebDataSource!)

Invoked when a data source finishes loading its content.

**Required**

Deprecated

