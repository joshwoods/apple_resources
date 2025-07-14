

- WatchKit
-  WKInterfaceScrollPosition 

Enumeration

# WKInterfaceScrollPosition

Onscreen scroll positions.

watchOS 4.0+

``` source
enum WKInterfaceScrollPosition
```

## Topics

### Enumeration Cases

case bottom

The bottom of the screen.

case centeredVertically

The vertical center of the screen.

case top

The top of the screen.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Scrolling

func scroll(to: WKInterfaceObject, at: WKInterfaceScrollPosition, animated: Bool)

Scrolls the specified object to the given position onscreen.

func interfaceDidScrollToTop()

Tells the interface controller that the user has performed a scroll-to-top gesture (for example, tapping the status bar) and that the scrolling animation has finished.

func interfaceOffsetDidScrollToTop()

Tells the interface controller that the user has scrolled to the top of the interface and that the scrolling animation has finished.

func interfaceOffsetDidScrollToBottom()

Tells the interface controller that the user has scrolled to the bottom of the interface and that the scrolling animation has finished.

var isTableScrollingHapticFeedbackEnabled: Bool

A Boolean value that determines whether haptic feedback coordinates with the appearance of new rows as the user scrolls through a table.

