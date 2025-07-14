

- AppKit
- NSStackView
-  insertView(\_:at:in:) 

Instance Method

# insertView(\_:at:in:)

Adds a view to a stack view gravity area at a specified index position.

macOS

``` source
@MainActor
func insertView(
    _ view: NSView,
    at index: Int,
    in gravity: NSStackView.Gravity
)
```

## Parameters 

`view`  

The view to add to the specified gravity area.

`index`  

The index position, within the gravity area, for the new view. The position of index `0` depends on the stack view layout direction and, for a horizontal stack view, on the user interface layout direction:

- *Horizontal*: The `0` index for a gravity area is at the leading side, as determined by the value of the inherited userInterfaceLayoutDirection property of the stack view. For a left to right language, index `0` is at the left of the gravity area.

- *Vertical*: The `0` index for a gravity area is at the top.

See the userInterfaceLayoutDirection property and the userInterfaceLayoutDirection method.

Important

If you specify an out-of-bounds value for the `index` parameter, the system raises an rangeException exception.

`gravity`  

The gravity area that you are adding the specified view to. Valid values are those in the NSStackView.Gravity enumeration.

## Discussion

Calling this method updates the stack view’s layout, which can change the stack view size. As a result, views could detach or clip according to the clipping resistance of the stack view and the visibility priorities of its views.

A view in a detached state is not present in the stack view’s view hierarchy, but it still consumes memory. To respond to detachment and reattachment of views, implement an NSStackViewDelegate object and assign it to the delegate property.

## See Also

### Related Documentation

func setVisibilityPriority(NSStackView.VisibilityPriority, for: NSView)

Sets the Auto Layout priority for a view to remain attached to the stack view when Auto Layout reduces the stack view’s size.

var orientation: NSUserInterfaceLayoutOrientation

The horizontal or vertical layout direction of the stack view.

func setClippingResistancePriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the Auto Layout priority for resisting clipping of views in the stack view when Auto Layout attempts to reduce the stack view’s size.

### Managing Views in Gravity Areas

func addView(NSView, in: NSStackView.Gravity)

Adds a view to the end of the stack view gravity area.

func setViews([NSView], in: NSStackView.Gravity)

Specifies an array of views for a specified gravity area in the stack view, replacing any previous views in that area.

func removeView(NSView)

Removes a specified view from the stack view.

enum Gravity

The gravity areas available in a stack view.

