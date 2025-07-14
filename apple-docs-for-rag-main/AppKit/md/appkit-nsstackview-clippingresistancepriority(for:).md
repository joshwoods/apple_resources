

- AppKit
- NSStackView
-  clippingResistancePriority(for:) 

Instance Method

# clippingResistancePriority(for:)

Returns the Auto Layout priority for resisting clipping of views in the stack view when Auto Layout attempts to reduce the stack view’s size.

macOS 10.9+

``` source
@MainActor
func clippingResistancePriority(for orientation: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority
```

## Parameters 

`orientation`  

The stack view layout direction to which the clipping resistance priority applies.

## Return Value

A layout constraint priority that identifies the clipping resistance for the stack view.

## Discussion

For an explanation of clipping resistance and how to use it for a stack view, see the setClippingResistancePriority(_:for:) method.

## See Also

### Related Documentation

var orientation: NSUserInterfaceLayoutOrientation

The horizontal or vertical layout direction of the stack view.

func setClippingResistancePriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the Auto Layout priority for resisting clipping of views in the stack view when Auto Layout attempts to reduce the stack view’s size.

### Inspecting a Stack View

var views: [NSView]

The array of views owned by the stack view.

func views(in: NSStackView.Gravity) -> [NSView]

Returns the array of views in the specified gravity area in the stack view.

var detachedViews: [NSView]

An array that contains the detached views from all the stack view’s gravity areas.

func huggingPriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the Auto Layout priority for the stack view to minimize its size to fit its contained views as closely as possible, for a specified user interface axis.

