

- WebKit
- WebDocumentRepresentation
-  canProvideDocumentSource() Deprecated

Instance Method

# canProvideDocumentSource()

Returns whether the receiver can provide content source.

macOS 10.3–10.14Deprecated

``` source
func canProvideDocumentSource() -> Bool
```

**Required**

## Return Value

true if the receiver can provide source for the document content (for example, HTML source), false otherwise.

## Discussion

The receiver should return true only if it makes sense for someone to view the source of the document in question. For example, a web view returns false if the content is an image, was produced by a plug-in, or contains text content already.

## See Also

### Getting document source

func documentSource() -> String!

Returns the receiver’s source as text.

**Required**

Deprecated

