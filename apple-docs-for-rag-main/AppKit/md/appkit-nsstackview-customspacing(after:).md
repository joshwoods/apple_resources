

- AppKit
- NSStackView
-  customSpacing(after:) 

Instance Method

# customSpacing(after:)

Returns the custom spacing, in points, between a specified view in the stack view and the view that follows it.

macOS 10.9+

``` source
@MainActor
func customSpacing(after view: NSView) -> CGFloat
```

## Parameters 

`view`  

The view whose trailing spacing you are getting.

## Return Value

The number of points between the trailing edge of the specified view and the one that follows it (that is, the one with the next highest index order).

## Discussion

If you set custom spacing for a view using the setCustomSpacing(_:after:) method, it overrides the stack view’s default spacing as set in the spacing property.

A stack view retains custom spacing across layout updates. Custom spacing for a view is lost if you remove the view from the stack view or specify a new value.

## See Also

### Configuring Views in a Stack View

func setCustomSpacing(CGFloat, after: NSView)

Specifies the custom spacing, in points, between a specified view and the view that follows it in the stack view.

func visibilityPriority(for: NSView) -> NSStackView.VisibilityPriority

Returns the visibility priority for a specified view in the stack view.

func setVisibilityPriority(NSStackView.VisibilityPriority, for: NSView)

Sets the Auto Layout priority for a view to remain attached to the stack view when Auto Layout reduces the stack view’s size.

struct VisibilityPriority

The various Auto Layout priorities for a view in the stack view to remain attached.

class let useDefaultSpacing: CGFloat

