

- WebKit
- WebDocumentRepresentation
-  receivedError(\_:with:) Deprecated

Instance Method

# receivedError(\_:with:)

Invoked when a data source receives an error loading its content.

macOS 10.3–10.14Deprecated

``` source
func receivedError(
    _ error: (any Error)!,
    with dataSource: WebDataSource!
)
```

**Required**

## Parameters 

`error`  

An `NSError` object that indicates what error occurred.

`dataSource`  

A `WebDataSource` object that identifies the request that caused this error.

## Discussion

The `error` argument contains details on the error that occurred.

## See Also

### Loading content

func receivedData(Data!, with: WebDataSource!)

Invoked when a data source has received some data.

**Required**

Deprecated

func finishedLoading(with: WebDataSource!)

Invoked when a data source finishes loading its content.

**Required**

Deprecated

