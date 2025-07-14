

- WatchKit
- WKInterfaceController
-  scroll(to:at:animated:) 

Instance Method

# scroll(to:at:animated:)

Scrolls the specified object to the given position onscreen.

watchOS 4.0+

``` source
@MainActor
func scroll(
    to object: WKInterfaceObject,
    at scrollPosition: WKInterfaceScrollPosition,
    animated: Bool
)
```

## Parameters 

`object`  

The interface object to scroll to.

`scrollPosition`  

The specified object’s desired position on the screen.

`animated`  

A Boolean value that determines whether the scroll action is animated.

## See Also

### Managing Scrolling

enum WKInterfaceScrollPosition

Onscreen scroll positions.

func interfaceDidScrollToTop()

Tells the interface controller that the user has performed a scroll-to-top gesture (for example, tapping the status bar) and that the scrolling animation has finished.

func interfaceOffsetDidScrollToTop()

Tells the interface controller that the user has scrolled to the top of the interface and that the scrolling animation has finished.

func interfaceOffsetDidScrollToBottom()

Tells the interface controller that the user has scrolled to the bottom of the interface and that the scrolling animation has finished.

var isTableScrollingHapticFeedbackEnabled: Bool

A Boolean value that determines whether haptic feedback coordinates with the appearance of new rows as the user scrolls through a table.

