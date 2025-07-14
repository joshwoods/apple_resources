

- PDFKit
- PDFDocument
-  selectionForEntireDocument 

Instance Property

# selectionForEntireDocument

Returns a selection representing the textual content of the entire document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var selectionForEntireDocument: PDFSelection? { get }
```

## See Also

### Working with Selections and Searches

func selection(from: PDFPage, atCharacterIndex: Int, to: PDFPage, atCharacterIndex: Int) -> PDFSelection?

Returns the specified selection based on starting and ending character indexes.

func selection(from: PDFPage, at: CGPoint, to: PDFPage, at: CGPoint) -> PDFSelection?

Returns the specified selection based on starting and ending points.

Search Operations

Find and search in PDFs.

