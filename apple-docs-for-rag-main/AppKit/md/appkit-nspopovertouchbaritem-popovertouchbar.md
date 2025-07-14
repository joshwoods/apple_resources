

- AppKit
- NSPopoverTouchBarItem
-  popoverTouchBar 

Instance Property

# popoverTouchBar

The bar displayed when this item is “popped.”

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var popoverTouchBar: NSTouchBar { get set }
```

## Discussion

Set this property to a fully configured instance of NSTouchBar that is displayed when the user taps on the popover item. By default this is an empty bar.

## See Also

### Configuring the expanded popover

var showsCloseButton: Bool

A Boolean value that determines whether a close button should be shown on the popover bar.

var pressAndHoldTouchBar: NSTouchBar?

The bar that is displayed when a user press-and-holds on the popover item.

