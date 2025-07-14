

- PDFKit
- PDFSelection
-  attributedString 

Instance Property

# attributedString

Returns an `NSAttributedString` object representing the text contained in the selection (may contain linefeed characters).

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var attributedString: NSAttributedString? { get }
```

## See Also

### Getting Information About a Selection

var pages: [PDFPage]

Returns the array of pages contained in the selection.

var string: String?

Returns an `NSString` object representing the text contained in the selection (may contain linefeed characters).

func bounds(for: PDFPage) -> CGRect

Returns the bounds of the selection on the specified page.

func selectionsByLine() -> [PDFSelection]

Returns an array of selections, one for each line of text covered by the receiver.

var color: UIColor?

Sets the color used for the drawing of a selection in both active and inactive states.

