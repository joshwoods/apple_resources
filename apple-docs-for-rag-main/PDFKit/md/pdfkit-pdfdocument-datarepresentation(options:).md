

- PDFKit
- PDFDocument
-  dataRepresentation(options:) 

Instance Method

# dataRepresentation(options:)

Returns a representation of the document as an `NSData` object with additional options applied, such as filters.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
func dataRepresentation(options: [AnyHashable : Any] = [:]) -> Data?
```

## See Also

### Creating Data Representations

func dataRepresentation() -> Data?

Returns a representation of the document as an `NSData` object.

