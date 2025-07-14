

- AppKit
- NSPopover
-  appearance 

Instance Property

# appearance

The appearance of the popover.

macOS 10.10+

``` source
@MainActor
var appearance: NSAppearance? { get set }
```

## Discussion

If no appearance is specified, the popover’s effective appearance defaults to vibrantLight.

In apps that run in macOS 10.10 and later, the previous property type of NSPopover.Appearance is deprecated. In apps that run in OS X v10.9 and earlier, the aqua appearance is automatically set on popover content.

## See Also

### Managing a Popover’s Appearance

var effectiveAppearance: NSAppearance

The appearance that will be used when the popover is displayed onscreen.

var animates: Bool

Specifies if the popover is to be animated.

var contentSize: NSSize

The content size of the popover.

var isShown: Bool

The display state of the popover.

var isDetached: Bool

A Boolean value that indicates whether the window created by a popover’s detachment is automatically created.

