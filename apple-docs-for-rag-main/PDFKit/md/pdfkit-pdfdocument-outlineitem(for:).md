

- PDFKit
- PDFDocument
-  outlineItem(for:) 

Instance Method

# outlineItem(for:)

Returns the most likely parent PDF outline object for the selection.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func outlineItem(for selection: PDFSelection) -> PDFOutline?
```

## Parameters 

`selection`  

The area of the document currently selected by the user. A selection can span multiple outline items, but only the point representing the first character is considered.

## Return Value

The PDF outline object that is the most likely parent of the specified selection. Note that only the point representing the first character of the selection is considered in this method.

## Discussion

Typically, outlines represent structural items such as chapters. You can use this method to identify the chapter that a selection falls within.

## See Also

### Accessing Document Information

var documentURL: URL?

The URL for the document.

var majorVersion: Int

The major version of the document.

var minorVersion: Int

The minor version of the document.

var string: String?

A string representing the textual content for the entire document.

var outlineRoot: PDFOutline?

The document’s root outline to a PDF outline object.

var documentAttributes: [AnyHashable : Any]?

A dictionary of document metadata.

var documentRef: CGPDFDocument?

The `CGPDFDocument` associated with the `PDFDocument` object.

