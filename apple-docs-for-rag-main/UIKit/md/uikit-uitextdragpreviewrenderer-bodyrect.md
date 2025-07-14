

- UIKit
- UITextDragPreviewRenderer
-  bodyRect 

Instance Property

# bodyRect

The bounding rectangle of the text in the middle of the drag preview.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var bodyRect: CGRect { get }
```

## Discussion

The body rectangle contains the full lines of text in the middle of the drag preview that doesn’t include the first line and last line. This property can be a zero rectangle. The initial value is also not calculated until the first time it’s used.

## See Also

### Getting and setting bounding rectangles

var firstLineRect: CGRect

The bounding rectangle of the first line of text in the drag preview.

var lastLineRect: CGRect

The bounding rectangle of the last line of text in the drag preview.

func adjust(firstLineRect: UnsafeMutablePointer&lt;CGRect>, bodyRect: UnsafeMutablePointer&lt;CGRect>, lastLineRect: UnsafeMutablePointer&lt;CGRect>, textOrigin: CGPoint)

Adjusts the size and origin of the bounding rectangles during a text drag operation.

