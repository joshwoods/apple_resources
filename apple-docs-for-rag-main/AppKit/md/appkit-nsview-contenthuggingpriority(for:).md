

- AppKit
- NSView
-  contentHuggingPriority(for:) 

Instance Method

# contentHuggingPriority(for:)

Returns the priority with which a view resists being made larger than its intrinsic size.

macOS 10.7+

``` source
@MainActor
func contentHuggingPriority(for orientation: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority
```

## Parameters 

`orientation`  

The orientation of the dimension of the view that might be enlarged.

## Return Value

The priority with which the view should resist being enlarged from its intrinsic size in the specified orientation.

## Discussion

The constraint-based layout system uses these priorities when determining the best layout for views that are encountering constraints that would require them to be larger than their intrinsic size.

Subclasses should not override this method. Instead, custom views should set default values for their content on creation, typically to defaultLow or defaultHigh.

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

func setContentHuggingPriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the priority with which a view resists being made larger than its intrinsic size.

class let noIntrinsicMetric: CGFloat

A value that tells the layout system to ignore the intrinsic size value for a given dimension.

