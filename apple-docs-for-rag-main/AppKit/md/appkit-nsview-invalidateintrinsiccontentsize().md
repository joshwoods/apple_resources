

- AppKit
- NSView
-  invalidateIntrinsicContentSize() 

Instance Method

# invalidateIntrinsicContentSize()

Invalidates the view’s intrinsic content size.

macOS 10.7+

``` source
@MainActor
func invalidateIntrinsicContentSize()
```

## Discussion

Call this when something changes in your custom view that invalidates its intrinsic content size. This allows the constraint-based layout system to take the new intrinsic content size into account in its next layout pass.

## See Also

### Measuring in Auto Layout

var fittingSize: NSSize

The minimum size of the view that satisfies the constraints it holds.

var intrinsicContentSize: NSSize

The natural size for the receiving view, considering only properties of the view itself.

func contentCompressionResistancePriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the priority with which a view resists being made smaller than its intrinsic size.

func setContentCompressionResistancePriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the priority with which a view resists being made smaller than its intrinsic size.

func contentHuggingPriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the priority with which a view resists being made larger than its intrinsic size.

func setContentHuggingPriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the priority with which a view resists being made larger than its intrinsic size.

class let noIntrinsicMetric: CGFloat

A value that tells the layout system to ignore the intrinsic size value for a given dimension.

