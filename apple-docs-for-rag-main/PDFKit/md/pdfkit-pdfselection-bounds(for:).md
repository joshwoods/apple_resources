

- PDFKit
- PDFSelection
-  bounds(for:) 

Instance Method

# bounds(for:)

Returns the bounds of the selection on the specified page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func bounds(for page: PDFPage) -> CGRect
```

**macOS**

``` source
func bounds(for page: PDFPage) -> NSRect
```

## Discussion

The selection rectangle is given in page space.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Getting Information About a Selection

var pages: [PDFPage]

Returns the array of pages contained in the selection.

var string: String?

Returns an `NSString` object representing the text contained in the selection (may contain linefeed characters).

var attributedString: NSAttributedString?

Returns an `NSAttributedString` object representing the text contained in the selection (may contain linefeed characters).

func selectionsByLine() -> [PDFSelection]

Returns an array of selections, one for each line of text covered by the receiver.

var color: UIColor?

Sets the color used for the drawing of a selection in both active and inactive states.

