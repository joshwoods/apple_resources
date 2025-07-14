

- PDFKit
- PDFSelection
-  selectionsByLine() 

Instance Method

# selectionsByLine()

Returns an array of selections, one for each line of text covered by the receiver.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
func selectionsByLine() -> [PDFSelection]
```

## Discussion

If you call this method on a `PDFSelection` object that represents a paragraph, for example, `selectionsByLine` returns an array that contains one `PDFSelection` object for each line of text in the paragraph.

## See Also

### Getting Information About a Selection

var pages: [PDFPage]

Returns the array of pages contained in the selection.

var string: String?

Returns an `NSString` object representing the text contained in the selection (may contain linefeed characters).

var attributedString: NSAttributedString?

Returns an `NSAttributedString` object representing the text contained in the selection (may contain linefeed characters).

func bounds(for: PDFPage) -> CGRect

Returns the bounds of the selection on the specified page.

var color: UIColor?

Sets the color used for the drawing of a selection in both active and inactive states.

