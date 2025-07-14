

- WatchKit
- WKInterfaceController
-  interfaceOffsetDidScrollToTop() 

Instance Method

# interfaceOffsetDidScrollToTop()

Tells the interface controller that the user has scrolled to the top of the interface and that the scrolling animation has finished.

watchOS 4.0+

``` source
@MainActor
func interfaceOffsetDidScrollToTop()
```

## Discussion

The default implementation of this method does nothing. You can override this method to take actions when the user scrolls to the top of the interface.

## See Also

### Managing Scrolling

func scroll(to: WKInterfaceObject, at: WKInterfaceScrollPosition, animated: Bool)

Scrolls the specified object to the given position onscreen.

enum WKInterfaceScrollPosition

Onscreen scroll positions.

func interfaceDidScrollToTop()

Tells the interface controller that the user has performed a scroll-to-top gesture (for example, tapping the status bar) and that the scrolling animation has finished.

func interfaceOffsetDidScrollToBottom()

Tells the interface controller that the user has scrolled to the bottom of the interface and that the scrolling animation has finished.

var isTableScrollingHapticFeedbackEnabled: Bool

A Boolean value that determines whether haptic feedback coordinates with the appearance of new rows as the user scrolls through a table.

