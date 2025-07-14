

- AppKit
- NSWindow
-  deepestScreen 

Instance Property

# deepestScreen

The deepest screen the window is on (it may be split over several screens).

macOS

``` source
@MainActor
var deepestScreen: NSScreen? { get }
```

## Discussion

The value of this property is `nil` when the window is offscreen.

## See Also

### Accessing Screen Information

var screen: NSScreen?

The screen the window is on.

var displaysWhenScreenProfileChanges: Bool

A Boolean value that indicates whether the window context should be updated when the screen profile changes or when the window moves to a different screen.

