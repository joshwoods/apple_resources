

- AppKit
- NSStackView
-  huggingPriority(for:) 

Instance Method

# huggingPriority(for:)

Returns the Auto Layout priority for the stack view to minimize its size to fit its contained views as closely as possible, for a specified user interface axis.

macOS 10.9+

``` source
@MainActor
func huggingPriority(for orientation: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority
```

## Parameters 

`orientation`  

The user interface axis (horizontal or vertical) whose hugging priority you want to get from the stack view. Valid values are those in the NSUserInterfaceLayoutOrientation enumeration.

## Return Value

The Auto Layout priority for the stack view to minimize its size.

## See Also

### Related Documentation

func setHuggingPriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the Auto Layout priority for the stack view to minimize its size, for a specified user interface axis.

### Inspecting a Stack View

var views: [NSView]

The array of views owned by the stack view.

func views(in: NSStackView.Gravity) -> [NSView]

Returns the array of views in the specified gravity area in the stack view.

var detachedViews: [NSView]

An array that contains the detached views from all the stack view’s gravity areas.

func clippingResistancePriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the Auto Layout priority for resisting clipping of views in the stack view when Auto Layout attempts to reduce the stack view’s size.

