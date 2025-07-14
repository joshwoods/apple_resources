

- AppKit
- NSPopover
-  contentSize 

Instance Property

# contentSize

The content size of the popover.

macOS 10.7+

``` source
@MainActor
var contentSize: NSSize { get set }
```

## Discussion

The popover’s content size is set to match the size of the content view when the content view controller is set.

Changes to the content size of the popover will cause the popover to animate while it is shown if the animates property is true.

This property is exposed as a read-only binding.

## See Also

### Managing a Popover’s Appearance

var appearance: NSAppearance?

The appearance of the popover.

var effectiveAppearance: NSAppearance

The appearance that will be used when the popover is displayed onscreen.

var animates: Bool

Specifies if the popover is to be animated.

var isShown: Bool

The display state of the popover.

var isDetached: Bool

A Boolean value that indicates whether the window created by a popover’s detachment is automatically created.

