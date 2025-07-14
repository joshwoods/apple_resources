

- PDFKit
- PDFDocument
-  selection(from:atCharacterIndex:to:atCharacterIndex:) 

Instance Method

# selection(from:atCharacterIndex:to:atCharacterIndex:)

Returns the specified selection based on starting and ending character indexes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func selection(
    from startPage: PDFPage,
    atCharacterIndex startCharacter: Int,
    to endPage: PDFPage,
    atCharacterIndex endCharacter: Int
) -> PDFSelection?
```

## Discussion

The selection begins at `startChar` on `startPage` and ends at `endChar` on `endPage`. The starting and ending index values must be in the range of the number of characters (as returned by numberOfCharacters) within the respective `PDFPage` objects.

## See Also

### Working with Selections and Searches

func selection(from: PDFPage, at: CGPoint, to: PDFPage, at: CGPoint) -> PDFSelection?

Returns the specified selection based on starting and ending points.

var selectionForEntireDocument: PDFSelection?

Returns a selection representing the textual content of the entire document.

Search Operations

Find and search in PDFs.

