

- AppKit
- NSView
-  baselineOffsetFromBottom 

Instance Property

# baselineOffsetFromBottom

The distance (in points) between the bottom of the view’s alignment rectangle and its baseline.

macOS 10.7+

``` source
@MainActor
var baselineOffsetFromBottom: CGFloat { get }
```

## Discussion

The default value of this property is `0`. For views that contain text or other content whose layout benefits from having a custom baseline, you can override this property and provide the correct distance between the bottom of the view’s alignment rectangle and that baseline.

## See Also

### Aligning Views with Auto Layout

func alignmentRect(forFrame: NSRect) -> NSRect

Returns the view’s alignment rectangle for a given frame.

func frame(forAlignmentRect: NSRect) -> NSRect

Returns the view’s frame for a given alignment rectangle.

var alignmentRectInsets: NSEdgeInsets

The insets (in points) from the view’s frame that define its content rectangle.

var firstBaselineOffsetFromTop: CGFloat

The distance (in points) between the top of the view’s alignment rectangle and its topmost baseline.

var lastBaselineOffsetFromBottom: CGFloat

The distance (in points) between the bottom of the view’s alignment rectangle and its bottommost baseline.

