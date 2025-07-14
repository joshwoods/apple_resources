

- PDFKit
- PDFPage
-  selection(from:to:) 

Instance Method

# selection(from:to:)

Returns the text between the two specified points in page space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func selection(
    from startPoint: CGPoint,
    to endPoint: CGPoint
) -> PDFSelection?
```

**macOS**

``` source
func selection(
    from startPoint: NSPoint,
    to endPoint: NSPoint
) -> PDFSelection?
```

## Discussion

Either point may be the one closer to the start of the page. In determining the selection, the points are sorted first top to bottom and then left to right.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

To visualize the selection, picture the rectangle defined by `startPoint` and `endPoint`. The selection begins at the first character fully within the defined rectangle and closest to its upper-left corner. The selection ends at the last character fully within the defined rectangle and closest to its lower-right corner.

## See Also

### Working with Selections

func selection(for: CGRect) -> PDFSelection?

Returns the text enclosed within the specified rectangle, expressed in page (user) coordinates.

func selectionForWord(at: CGPoint) -> PDFSelection?

Returns the whole word that includes the specified point.

func selectionForLine(at: CGPoint) -> PDFSelection?

Returns the whole line of text that includes the specified point.

func selection(for: NSRange) -> PDFSelection?

Returns the text contained within the specified range.

