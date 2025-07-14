

- AppKit
- NSView
-  noIntrinsicMetric 

Type Property

# noIntrinsicMetric

A value that tells the layout system to ignore the intrinsic size value for a given dimension.

macOS 10.11+

``` source
class let noIntrinsicMetric: CGFloat
```

## Discussion

Specify this value if a view doesn’t have an intrinsic height or width. For example, a horizontal slider has an intrinsic height but might have no intrinsic width.

## See Also

### Measuring in Auto Layout

var fittingSize: NSSize

The minimum size of the view that satisfies the constraints it holds.

var intrinsicContentSize: NSSize

The natural size for the receiving view, considering only properties of the view itself.

func invalidateIntrinsicContentSize()

Invalidates the view’s intrinsic content size.

func contentCompressionResistancePriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the priority with which a view resists being made smaller than its intrinsic size.

func setContentCompressionResistancePriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the priority with which a view resists being made smaller than its intrinsic size.

func contentHuggingPriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the priority with which a view resists being made larger than its intrinsic size.

func setContentHuggingPriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the priority with which a view resists being made larger than its intrinsic size.

