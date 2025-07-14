

- AppKit
- NSView
-  frame(forAlignmentRect:) 

Instance Method

# frame(forAlignmentRect:)

Returns the view’s frame for a given alignment rectangle.

macOS 10.7+

``` source
@MainActor
func frame(forAlignmentRect alignmentRect: NSRect) -> NSRect
```

## Parameters 

`alignmentRect`  

The alignment rectangle whose corresponding frame is desired.

## Return Value

The frame for the specified alignment rectangle

## Discussion

The constraint-based layout system uses alignment rectangles to align views, rather than their frame. This allows custom views to be aligned based on the location of their content while still having a frame that encompasses any ornamentation they need to draw around their content, such as shadows or reflections.

The default implementation returns `alignmentRect` modified by the insets specified by the view’s alignmentRectInsets method. Most custom views can override alignmentRectInsets to specify the location of their content within their frame. Custom views that require arbitrary transformations can override alignmentRect(forFrame:) and frame(forAlignmentRect:) to describe the location of their content. These two methods must always be inverses of each other.

## See Also

### Aligning Views with Auto Layout

func alignmentRect(forFrame: NSRect) -> NSRect

Returns the view’s alignment rectangle for a given frame.

var alignmentRectInsets: NSEdgeInsets

The insets (in points) from the view’s frame that define its content rectangle.

var baselineOffsetFromBottom: CGFloat

The distance (in points) between the bottom of the view’s alignment rectangle and its baseline.

var firstBaselineOffsetFromTop: CGFloat

The distance (in points) between the top of the view’s alignment rectangle and its topmost baseline.

var lastBaselineOffsetFromBottom: CGFloat

The distance (in points) between the bottom of the view’s alignment rectangle and its bottommost baseline.

