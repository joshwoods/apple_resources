

- PDFKit
- PDFSelection
-  color 

Instance Property

# color

Sets the color used for the drawing of a selection in both active and inactive states.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
@NSCopying
var color: NSColor? { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@NSCopying
var color: UIColor? { get set }
```

## Discussion

When no color has been specified for the `PDFSelection` objects in a document, the selections are drawn using `[NSColor selectedTextBackgroundColor]` for the active state and `[NSColor secondarySelectedControlColor]` for the inactive state. Use the `setColor` method to supply a color you want to be used for the drawing of both active and inactive selections.

## See Also

### Related Documentation

class PDFSelection

A `PDFSelection` object identifies a contiguous or noncontiguous selection of text in a PDF document.

### Getting Information About a Selection

var pages: [PDFPage]

Returns the array of pages contained in the selection.

var string: String?

Returns an `NSString` object representing the text contained in the selection (may contain linefeed characters).

var attributedString: NSAttributedString?

Returns an `NSAttributedString` object representing the text contained in the selection (may contain linefeed characters).

func bounds(for: PDFPage) -> CGRect

Returns the bounds of the selection on the specified page.

func selectionsByLine() -> [PDFSelection]

Returns an array of selections, one for each line of text covered by the receiver.

