

- PDFKit
- PDFDocument
-  write(toFile:withOptions:) 

Instance Method

# write(toFile:withOptions:)

Writes the document to a file at the specified path with the specified options.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func write(
    toFile path: String,
    withOptions options: [PDFDocumentWriteOption : Any]? = nil
) -> Bool
```

## Discussion

The most commonly-used options are `kCGPDFContextOwnerPassword`, `kCGPDFContextUserPassword`, `kCGPDFContextAllowsCopying` and `kCGPDFContextAllowsPrinting`. For more details about these options, see the “Auxiliary Dictionary Keys” in doc://com.apple.documentation/documentation/coregraphics/cgpdfcontext, part of the Quartz 2D Reference.

## See Also

### Related Documentation

func dataRepresentation() -> Data?

Returns a representation of the document as an `NSData` object.

### Writing Out the PDF Data

func write(toFile: String) -> Bool

Writes the document to a file at the specified path.

func write(to: URL) -> Bool

Writes the document to a location specified by the passed-in URL.

func write(to: URL, withOptions: [PDFDocumentWriteOption : Any]?) -> Bool

Writes the document to the specified URL with the specified options.

Data Representations

Operations to represent PDF documents as data objects.

