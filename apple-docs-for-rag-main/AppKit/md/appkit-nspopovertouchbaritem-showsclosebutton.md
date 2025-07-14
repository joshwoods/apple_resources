

- AppKit
- NSPopoverTouchBarItem
-  showsCloseButton 

Instance Property

# showsCloseButton

A Boolean value that determines whether a close button should be shown on the popover bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var showsCloseButton: Bool { get set }
```

## Discussion

When true, a close button is automatically displayed when the popover bar is displayed. When false, it is your responsibility to dismiss the popover bar.

## See Also

### Configuring the expanded popover

var popoverTouchBar: NSTouchBar

The bar displayed when this item is “popped.”

var pressAndHoldTouchBar: NSTouchBar?

The bar that is displayed when a user press-and-holds on the popover item.

