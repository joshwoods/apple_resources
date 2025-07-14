

- AppKit
- NSStackView
-  detachedViews 

Instance Property

# detachedViews

An array that contains the detached views from all the stack view’s gravity areas.

macOS 10.9+

``` source
@MainActor
var detachedViews: [NSView] { get }
```

## Discussion

A view in a detached state is not present in the stack view’s view hierarchy, but it still consumes memory.

Note

There is no guaranteed ordering of the views in the detached views array.

## See Also

### Inspecting a Stack View

var views: [NSView]

The array of views owned by the stack view.

func views(in: NSStackView.Gravity) -> [NSView]

Returns the array of views in the specified gravity area in the stack view.

func clippingResistancePriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the Auto Layout priority for resisting clipping of views in the stack view when Auto Layout attempts to reduce the stack view’s size.

func huggingPriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the Auto Layout priority for the stack view to minimize its size to fit its contained views as closely as possible, for a specified user interface axis.

