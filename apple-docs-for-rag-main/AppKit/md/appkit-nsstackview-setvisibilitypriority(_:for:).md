

- AppKit
- NSStackView
-  setVisibilityPriority(\_:for:) 

Instance Method

# setVisibilityPriority(\_:for:)

Sets the Auto Layout priority for a view to remain attached to the stack view when Auto Layout reduces the stack view’s size.

macOS 10.9+

``` source
@MainActor
func setVisibilityPriority(
    _ priority: NSStackView.VisibilityPriority,
    for view: NSView
)
```

## Parameters 

`priority`  

The visibility priority for a specified view. Valid values are those in the NSStackView.VisibilityPriority enumeration.

`view`  

The view whose visibility priority you are setting.

Important

If you attempt to set visibility priority for a view that is not in the stack view, the system raises an exception.

## Discussion

When Auto Layout reduces the stack view’s size (such as when a user reduces the size of the window containing the stack view), causing one or more views to no longer fit, the stack view detaches views in order of increasing *visibility priority*. A view with lower visibility priority detaches before a view with higher visibility priority. A set of views with identical, detachable visibility priority are all detached or reattached together. A view with the highest possible visibility priority never detaches.

A view in a detached state is not present in the stack view’s view hierarchy, but it still consumes memory.

The default visibility priority for a view is mustHold, resulting in the view never detaching.

To allow a view to detach as needed by the stack view, set a visibility priority of detachOnlyIfNecessary. To force a view to detach regardless of the enclosing view’s size, set a visibility priority of notVisible. To explicitly reattach a view to a stack view, set a visibility priority of mustHold.

## See Also

### Configuring Views in a Stack View

func customSpacing(after: NSView) -> CGFloat

Returns the custom spacing, in points, between a specified view in the stack view and the view that follows it.

func setCustomSpacing(CGFloat, after: NSView)

Specifies the custom spacing, in points, between a specified view and the view that follows it in the stack view.

func visibilityPriority(for: NSView) -> NSStackView.VisibilityPriority

Returns the visibility priority for a specified view in the stack view.

struct VisibilityPriority

The various Auto Layout priorities for a view in the stack view to remain attached.

class let useDefaultSpacing: CGFloat

