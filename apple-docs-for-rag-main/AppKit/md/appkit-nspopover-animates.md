

- AppKit
- NSPopover
-  animates 

Instance Property

# animates

Specifies if the popover is to be animated.

macOS 10.7+

``` source
@MainActor
var animates: Bool { get set }
```

## Discussion

A popover may be animated when it shows, closes, moves, or appears to transition to a detachable window. This property also controls whether the popover animates when the content view or content size changes.

The system does not guarantee which behaviors will be animated or that this property will be respected; it is regarded as a hint.

The default value is true.

## See Also

### Managing a Popover’s Appearance

var appearance: NSAppearance?

The appearance of the popover.

var effectiveAppearance: NSAppearance

The appearance that will be used when the popover is displayed onscreen.

var contentSize: NSSize

The content size of the popover.

var isShown: Bool

The display state of the popover.

var isDetached: Bool

A Boolean value that indicates whether the window created by a popover’s detachment is automatically created.

