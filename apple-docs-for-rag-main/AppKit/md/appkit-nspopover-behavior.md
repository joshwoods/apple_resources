

- AppKit
- NSPopover
-  behavior 

Instance Property

# behavior

Specifies the behavior of the popover.

macOS 10.7+

``` source
@MainActor
var behavior: NSPopover.Behavior { get set }
```

## Discussion

The default value is NSPopover.Behavior.applicationDefined. See NSPopover.Behavior for possible value.

## See Also

### Managing a Popover’s Position and Size

func show(relativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge)

Shows the popover anchored to the specified view.

var positioningRect: NSRect

The rectangle within the positioning view relative to which the popover should be positioned.

