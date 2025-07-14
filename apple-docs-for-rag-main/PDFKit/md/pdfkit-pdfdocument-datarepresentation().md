

- PDFKit
- PDFDocument
-  dataRepresentation() 

Instance Method

# dataRepresentation()

Returns a representation of the document as an `NSData` object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func dataRepresentation() -> Data?
```

## See Also

### Related Documentation

func write(toFile: String) -> Bool

Writes the document to a file at the specified path.

func write(to: URL) -> Bool

Writes the document to a location specified by the passed-in URL.

### Creating Data Representations

func dataRepresentation(options: [AnyHashable : Any]) -> Data?

Returns a representation of the document as an `NSData` object with additional options applied, such as filters.

