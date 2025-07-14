

- PDFKit
- PDFDocument
-  write(to:withOptions:) 

Instance Method

# write(to:withOptions:)

Writes the document to the specified URL with the specified options.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func write(
    to url: URL,
    withOptions options: [PDFDocumentWriteOption : Any]? = nil
) -> Bool
```

## See Also

### Related Documentation

func dataRepresentation() -> Data?

Returns a representation of the document as an `NSData` object.

### Writing Out the PDF Data

func write(toFile: String) -> Bool

Writes the document to a file at the specified path.

func write(toFile: String, withOptions: [PDFDocumentWriteOption : Any]?) -> Bool

Writes the document to a file at the specified path with the specified options.

func write(to: URL) -> Bool

Writes the document to a location specified by the passed-in URL.

Data Representations

Operations to represent PDF documents as data objects.

