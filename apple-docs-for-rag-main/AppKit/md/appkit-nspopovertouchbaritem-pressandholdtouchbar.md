

- AppKit
- NSPopoverTouchBarItem
-  pressAndHoldTouchBar 

Instance Property

# pressAndHoldTouchBar

The bar that is displayed when a user press-and-holds on the popover item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var pressAndHoldTouchBar: NSTouchBar? { get set }
```

## Discussion

This NSTouchBar can be the same as the one used for the popoverTouchBar property, but does not have to be.

When non-`nil` this touch bar is displayed while the user holds their finger down on the collapsed representation of the popover item. When the user raises their finger, this bar disappears.

## See Also

### Configuring the expanded popover

var popoverTouchBar: NSTouchBar

The bar displayed when this item is “popped.”

var showsCloseButton: Bool

A Boolean value that determines whether a close button should be shown on the popover bar.

