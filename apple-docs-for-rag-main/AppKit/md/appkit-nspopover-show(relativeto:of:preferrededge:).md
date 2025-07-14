

- AppKit
- NSPopover
-  show(relativeTo:of:preferredEdge:) 

Instance Method

# show(relativeTo:of:preferredEdge:)

Shows the popover anchored to the specified view.

macOS 10.7+

``` source
@MainActor
func show(
    relativeTo positioningRect: NSRect,
    of positioningView: NSView,
    preferredEdge: NSRectEdge
)
```

## Parameters 

`positioningRect`  

The rectangle within `positioningView` relative to which the popover should be positioned. Normally set to the bounds of `positioningView`. May be an empty rectangle, which will default to the bounds of `positioningView`.

`positioningView`  

The view relative to which the popover should be positioned. Causes the method to raise invalidArgumentException if `nil`.

`preferredEdge`  

The edge of `positioningView` the popover should prefer to be anchored to.

## Discussion

This method raises internalInconsistencyException if contentViewController or the view controller’s view is `nil`. If the popover is already being shown, this method updates the anchored view, rectangle, and preferred edge. If the positioning view is not visible, this method does nothing.

## See Also

### Managing a Popover’s Position and Size

var behavior: NSPopover.Behavior

Specifies the behavior of the popover.

var positioningRect: NSRect

The rectangle within the positioning view relative to which the popover should be positioned.

