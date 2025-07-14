

- AppKit
- NSPopover
-  isDetached 

Instance Property

# isDetached

A Boolean value that indicates whether the window created by a popover’s detachment is automatically created.

macOS 10.10+

``` source
@MainActor
var isDetached: Bool { get }
```

## Discussion

When isDetached is true, the detached window is automatically created. This property does not apply when detaching a popover results in a window returned by detachableWindow(for:).

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

var isShown: Bool

The display state of the popover.

