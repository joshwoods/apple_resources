

- AppKit
- NSWindow
-  displaysWhenScreenProfileChanges 

Instance Property

# displaysWhenScreenProfileChanges

A Boolean value that indicates whether the window context should be updated when the screen profile changes or when the window moves to a different screen.

macOS

``` source
@MainActor
var displaysWhenScreenProfileChanges: Bool { get set }
```

## Discussion

The value of this property is true when the window context should be updated when the ColorSync profile of the current screen changes or when a majority of the window is moved to a different screen whose profile is different than the previous screen; otherwise, false. The default value is false.

After the window context is updated, the window is told to display itself. If you need to update offscreen caches for the window, you should register to receive the didChangeScreenProfileNotification notification.

## See Also

### Accessing Screen Information

var screen: NSScreen?

The screen the window is on.

var deepestScreen: NSScreen?

The deepest screen the window is on (it may be split over several screens).

