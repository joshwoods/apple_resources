

- AppKit
- NSStackView
-  visibilityPriority(for:) 

Instance Method

# visibilityPriority(for:)

Returns the visibility priority for a specified view in the stack view.

macOS 10.9+

``` source
@MainActor
func visibilityPriority(for view: NSView) -> NSStackView.VisibilityPriority
```

## Parameters 

`view`  

The view that you are getting the visibility priority for.

## Return Value

The visibility priority for the specified view.

## Discussion

Visibility priority is the Auto Layout priority for a view to remain attached to a stack view when Auto Layout reduces the stack view’s size (such as when a user reduces the enclosing window’s size).

## See Also

### Configuring Views in a Stack View

func customSpacing(after: NSView) -> CGFloat

Returns the custom spacing, in points, between a specified view in the stack view and the view that follows it.

func setCustomSpacing(CGFloat, after: NSView)

Specifies the custom spacing, in points, between a specified view and the view that follows it in the stack view.

func setVisibilityPriority(NSStackView.VisibilityPriority, for: NSView)

Sets the Auto Layout priority for a view to remain attached to the stack view when Auto Layout reduces the stack view’s size.

struct VisibilityPriority

The various Auto Layout priorities for a view in the stack view to remain attached.

class let useDefaultSpacing: CGFloat

