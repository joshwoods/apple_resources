

- PDFKit
- PDFDocument
-  selection(from:at:to:at:) 

Instance Method

# selection(from:at:to:at:)

Returns the specified selection based on starting and ending points.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
func selection(
    from startPage: PDFPage,
    at startPoint: NSPoint,
    to endPage: PDFPage,
    at endPoint: NSPoint
) -> PDFSelection?
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func selection(
    from startPage: PDFPage,
    at startPoint: CGPoint,
    to endPage: PDFPage,
    at endPoint: CGPoint
) -> PDFSelection?
```

## Discussion

The selection begins at `startPt` on `startPage` and ends at `endPt` on `endPage`. The starting and ending points should be specified in page space, relative to their respective pages.

The starting and ending points can be on the same page. In this case, invoking this method is equivalent to sending the `selectionFromPoint:toPoint:` message to a `PDFPage` object.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Related Documentation

func selection(for: NSRange) -> PDFSelection?

Returns the text contained within the specified range.

### Working with Selections and Searches

func selection(from: PDFPage, atCharacterIndex: Int, to: PDFPage, atCharacterIndex: Int) -> PDFSelection?

Returns the specified selection based on starting and ending character indexes.

var selectionForEntireDocument: PDFSelection?

Returns a selection representing the textual content of the entire document.

Search Operations

Find and search in PDFs.

