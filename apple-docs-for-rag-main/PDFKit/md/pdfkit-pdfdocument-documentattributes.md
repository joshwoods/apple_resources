

- PDFKit
- PDFDocument
-  documentAttributes 

Instance Property

# documentAttributes

A dictionary of document metadata.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var documentAttributes: [AnyHashable : Any]? { get set }
```

## Return Value

The dictionary of document metadata. The dictionary may be empty, or only some of the keys may have associated values.

## Discussion

Metadata is optional for PDF documents.

## See Also

### Related Documentation

struct PDFDocumentAttribute

A structure that specifies document attributes.

### Accessing Document Information

var documentURL: URL?

The URL for the document.

var majorVersion: Int

The major version of the document.

var minorVersion: Int

The minor version of the document.

var string: String?

A string representing the textual content for the entire document.

func outlineItem(for: PDFSelection) -> PDFOutline?

Returns the most likely parent PDF outline object for the selection.

var outlineRoot: PDFOutline?

The document’s root outline to a PDF outline object.

var documentRef: CGPDFDocument?

The `CGPDFDocument` associated with the `PDFDocument` object.

