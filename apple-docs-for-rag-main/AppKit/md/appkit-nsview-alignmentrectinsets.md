

- AppKit
- NSView
-  alignmentRectInsets 

Instance Property

# alignmentRectInsets

The insets (in points) from the view’s frame that define its content rectangle.

macOS 10.7+

``` source
@MainActor
var alignmentRectInsets: NSEdgeInsets { get }
```

## Discussion

The default value is an NSEdgeInsets structure with the value `0` for each component. Custom views that draw ornamentation around their content can override this property and return insets that align with the edges of the content, excluding the ornamentation. This allows the constraint-based layout system to align views based on their content, rather than just their frame.

Custom views whose content location can’t be expressed by a simple set of insets should override alignmentRect(forFrame:) and frame(forAlignmentRect:) to describe their custom transform between alignment rectangle and frame.

## See Also

### Aligning Views with Auto Layout

func alignmentRect(forFrame: NSRect) -> NSRect

Returns the view’s alignment rectangle for a given frame.

func frame(forAlignmentRect: NSRect) -> NSRect

Returns the view’s frame for a given alignment rectangle.

var baselineOffsetFromBottom: CGFloat

The distance (in points) between the bottom of the view’s alignment rectangle and its baseline.

var firstBaselineOffsetFromTop: CGFloat

The distance (in points) between the top of the view’s alignment rectangle and its topmost baseline.

var lastBaselineOffsetFromBottom: CGFloat

The distance (in points) between the bottom of the view’s alignment rectangle and its bottommost baseline.

