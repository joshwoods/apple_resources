

- AppKit
- NSPopover
-  positioningRect 

Instance Property

# positioningRect

The rectangle within the positioning view relative to which the popover should be positioned.

macOS 10.7+

``` source
@MainActor
var positioningRect: NSRect { get set }
```

## Discussion

Popovers are positioned relative to a positioning view and are automatically moved when the location or size of the positioning view changes.

Sometimes it is desirable to position popovers relative to a rectangle within the positioning view. In this case, you must update the `positioningRect` property whenever this rectangle changes.

This property is exposed as a read-only binding.

## See Also

### Managing a Popover’s Position and Size

var behavior: NSPopover.Behavior

Specifies the behavior of the popover.

func show(relativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge)

Shows the popover anchored to the specified view.

