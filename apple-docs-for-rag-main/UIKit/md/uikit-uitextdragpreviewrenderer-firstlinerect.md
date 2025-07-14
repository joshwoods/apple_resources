

- UIKit
- UITextDragPreviewRenderer
-  firstLineRect 

Instance Property

# firstLineRect

The bounding rectangle of the first line of text in the drag preview.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var firstLineRect: CGRect { get }
```

## Discussion

The first line rectangle contains the first line of text in the drag preview that may be a partial line. This property can be a zero rectangle. The initial value is also not calculated until the first time it’s used.

## See Also

### Getting and setting bounding rectangles

var bodyRect: CGRect

The bounding rectangle of the text in the middle of the drag preview.

var lastLineRect: CGRect

The bounding rectangle of the last line of text in the drag preview.

func adjust(firstLineRect: UnsafeMutablePointer&lt;CGRect>, bodyRect: UnsafeMutablePointer&lt;CGRect>, lastLineRect: UnsafeMutablePointer&lt;CGRect>, textOrigin: CGPoint)

Adjusts the size and origin of the bounding rectangles during a text drag operation.

