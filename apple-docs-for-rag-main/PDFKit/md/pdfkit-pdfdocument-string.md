

- PDFKit
- PDFDocument
-  string 

Instance Property

# string

A string representing the textual content for the entire document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var string: String? { get }
```

## Return Value

A string that represents the textual content of the entire document.

## Discussion

Pages are delimited with linefeed characters.

This is a convenience method, equivalent to creating a selection object for the entire document and then invoking the `PDFSelection` class’s string method.

## See Also

### Accessing Document Information

var documentURL: URL?

The URL for the document.

var majorVersion: Int

The major version of the document.

var minorVersion: Int

The minor version of the document.

func outlineItem(for: PDFSelection) -> PDFOutline?

Returns the most likely parent PDF outline object for the selection.

var outlineRoot: PDFOutline?

The document’s root outline to a PDF outline object.

var documentAttributes: [AnyHashable : Any]?

A dictionary of document metadata.

var documentRef: CGPDFDocument?

The `CGPDFDocument` associated with the `PDFDocument` object.

