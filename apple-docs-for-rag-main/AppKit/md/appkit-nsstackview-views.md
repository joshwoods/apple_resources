

- AppKit
- NSStackView
-  views 

Instance Property

# views

The array of views owned by the stack view.

macOS

``` source
@MainActor
var views: [NSView] { get }
```

## Discussion

The `views` array always contains all of the views owned and managed by the stack view, regardless of their gravity area placement and regardless of whether or not they are attached. The index position of each view in the array matches the view ordering within the stack view. A detached view’s index position is its stack view position when attached.

## See Also

### Inspecting a Stack View

func views(in: NSStackView.Gravity) -> [NSView]

Returns the array of views in the specified gravity area in the stack view.

var detachedViews: [NSView]

An array that contains the detached views from all the stack view’s gravity areas.

func clippingResistancePriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the Auto Layout priority for resisting clipping of views in the stack view when Auto Layout attempts to reduce the stack view’s size.

func huggingPriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the Auto Layout priority for the stack view to minimize its size to fit its contained views as closely as possible, for a specified user interface axis.

