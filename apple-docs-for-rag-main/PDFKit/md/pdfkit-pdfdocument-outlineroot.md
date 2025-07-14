

- PDFKit
- PDFDocument
-  outlineRoot 

Instance Property

# outlineRoot

The document’s root outline to a PDF outline object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
var outlineRoot: PDFOutline? { get set }
```

## Parameters 

`outline`  

The outline to be used as the document’s root outline. Pass `NULL` to strip the outline from a document.

## Discussion

When a PDF document is saved, the outline tree structure is written out to the destination PDF file.

## See Also

### Related Documentation

class PDFDocument

An object that represents PDF data or a PDF file and defines methods for writing, searching, and selecting PDF data.

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

var documentAttributes: [AnyHashable : Any]?

A dictionary of document metadata.

var documentRef: CGPDFDocument?

The `CGPDFDocument` associated with the `PDFDocument` object.

