

- AppKit
- NSStackView
-  setCustomSpacing(\_:after:) 

Instance Method

# setCustomSpacing(\_:after:)

Specifies the custom spacing, in points, between a specified view and the view that follows it in the stack view.

macOS 10.9+

``` source
@MainActor
func setCustomSpacing(
    _ spacing: CGFloat,
    after view: NSView
)
```

## Parameters 

`spacing`  

The custom trailing space to use between the `aView` view and the one that follows it, in points.

Default value is useDefaultSpacing, which indicates that the view does not use custom spacing.

`view`  

The view whose trailing spacing you are setting.

Important

If you attempt to set custom spacing for a view that is not in the stack view, the system raises an exception.

## Discussion

For a horizontal stack view, this method sets custom spacing between a specified view and the view to its right when the user interface direction is left to right. (See the inherited userInterfaceLayoutDirection property for information on layout direction.) For a vertical stack view, this method sets custom spacing below a specified view.

If you set custom spacing for a view, it overrides the stack view’s default spacing for that view, as set in the spacing property.

A stack view retains custom spacing across layout updates. Custom spacing for a view is lost if you remove the view from the stack view or specify a new value.

## See Also

### Related Documentation

var spacing: CGFloat

The minimum spacing, in points, between adjacent views in the stack view.

### Configuring Views in a Stack View

func customSpacing(after: NSView) -> CGFloat

Returns the custom spacing, in points, between a specified view in the stack view and the view that follows it.

func visibilityPriority(for: NSView) -> NSStackView.VisibilityPriority

Returns the visibility priority for a specified view in the stack view.

func setVisibilityPriority(NSStackView.VisibilityPriority, for: NSView)

Sets the Auto Layout priority for a view to remain attached to the stack view when Auto Layout reduces the stack view’s size.

struct VisibilityPriority

The various Auto Layout priorities for a view in the stack view to remain attached.

class let useDefaultSpacing: CGFloat

