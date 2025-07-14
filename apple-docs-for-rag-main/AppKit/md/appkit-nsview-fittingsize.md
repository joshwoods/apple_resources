

- AppKit
- NSView
-  fittingSize 

Instance Property

# fittingSize

The minimum size of the view that satisfies the constraints it holds.

macOS 10.7+

``` source
@MainActor
var fittingSize: NSSize { get }
```

## Discussion

AppKit sets this property to the best size available for the view, considering all of the constraints it and its subviews hold and satisfying a preference to make the view as small as possible. The size values in this property are never negative.

## See Also

### Measuring in Auto Layout

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

class let noIntrinsicMetric: CGFloat

A value that tells the layout system to ignore the intrinsic size value for a given dimension.

