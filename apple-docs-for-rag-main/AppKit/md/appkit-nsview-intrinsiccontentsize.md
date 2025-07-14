

- AppKit
- NSView
-  intrinsicContentSize 

Instance Property

# intrinsicContentSize

The natural size for the receiving view, considering only properties of the view itself.

macOS 10.7+

``` source
@MainActor
var intrinsicContentSize: NSSize { get }
```

## Return Value

A size indicating the natural size for the receiving view based on its intrinsic properties.

## Discussion

The default width and height values of this property are set to noIntrinsicMetric. For a custom view, you can override this property and use it to communicate what size you would like your view to be based on its content. You might do this in cases where the layout system cannot determine the size of the view based solely on its current constraints. For example, a text field might override this method and return an intrinsic size based on the text it contains. The intrinsic size you supply must be independent of the content frame, because there’s no way to dynamically communicate a changed width to the layout system based on a changed height. If your custom view has no intrinsic size for a given dimension, you can set the corresponding dimension to the noIntrinsicMetric.

## See Also

### Measuring in Auto Layout

var fittingSize: NSSize

The minimum size of the view that satisfies the constraints it holds.

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

