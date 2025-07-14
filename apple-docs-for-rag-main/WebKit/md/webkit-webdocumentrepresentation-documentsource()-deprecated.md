

- WebKit
- WebDocumentRepresentation
-  documentSource() Deprecated

Instance Method

# documentSource()

Returns the receiver’s source as text.

macOS 10.3–10.14Deprecated

``` source
func documentSource() -> String!
```

**Required**

## Return Value

Returns the document source associated with the receiver or `nil` if the source cannot be provided.

## Discussion

For example, for HTML documents, the receiver should return the HTML source.

## See Also

### Getting document source

func canProvideDocumentSource() -> Bool

Returns whether the receiver can provide content source.

**Required**

Deprecated

