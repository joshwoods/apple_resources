

- AppKit
- NSPopover
-  isShown 

Instance Property

# isShown

The display state of the popover.

macOS 10.7+

``` source
@MainActor
var isShown: Bool { get }
```

## Discussion

The value is true if the popover is being shown, false otherwise.

The popover is considered to be shown from the point when show(relativeTo:of:preferredEdge:) is invoked. A popover is considered closed in response to an invocation of either close() or performClose(_:).

## See Also

### Managing a Popover’s Appearance

var appearance: NSAppearance?

The appearance of the popover.

var effectiveAppearance: NSAppearance

The appearance that will be used when the popover is displayed onscreen.

var animates: Bool

Specifies if the popover is to be animated.

var contentSize: NSSize

The content size of the popover.

var isDetached: Bool

A Boolean value that indicates whether the window created by a popover’s detachment is automatically created.

