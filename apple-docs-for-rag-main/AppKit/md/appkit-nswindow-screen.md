

- AppKit
- NSWindow
-  screen 

Instance Property

# screen

The screen the window is on.

macOS

``` source
@MainActor
var screen: NSScreen? { get }
```

## Discussion

The value of this property is the screen where most of the window is on; it is `nil` when the window is offscreen.

## See Also

### Accessing Screen Information

var deepestScreen: NSScreen?

The deepest screen the window is on (it may be split over several screens).

var displaysWhenScreenProfileChanges: Bool

A Boolean value that indicates whether the window context should be updated when the screen profile changes or when the window moves to a different screen.

