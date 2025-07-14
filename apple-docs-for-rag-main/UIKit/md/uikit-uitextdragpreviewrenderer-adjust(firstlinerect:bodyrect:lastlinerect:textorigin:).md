

- UIKit
- UITextDragPreviewRenderer
-  adjust(firstLineRect:bodyRect:lastLineRect:textOrigin:) 

Instance Method

# adjust(firstLineRect:bodyRect:lastLineRect:textOrigin:)

Adjusts the size and origin of the bounding rectangles during a text drag operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func adjust(
    firstLineRect: UnsafeMutablePointer,
    bodyRect: UnsafeMutablePointer,
    lastLineRect: UnsafeMutablePointer,
    textOrigin origin: CGPoint
)
```

## Parameters 

`firstLineRect`  

The bounding rectangle for the first line of text in the drag preview.

`bodyRect`  

The bounding rectangle for the text in the middle of the drag preview that doesn’t include the first and last line.

`lastLineRect`  

The bounding rectangle for the last line of text in the drag preview.

`origin`  

The origin of the text preview.

## Discussion

This method does nothing by default. Subclasses may override this method to change the rectangle calculations; for example, in order to enlarge the rectangles by a few points. If you adjust the rectangles, the drag preview changes accordingly.

## See Also

### Getting and setting bounding rectangles

var bodyRect: CGRect

The bounding rectangle of the text in the middle of the drag preview.

var firstLineRect: CGRect

The bounding rectangle of the first line of text in the drag preview.

var lastLineRect: CGRect

The bounding rectangle of the last line of text in the drag preview.

