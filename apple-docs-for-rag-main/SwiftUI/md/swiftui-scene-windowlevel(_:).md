

- SwiftUI
- Scene
-  windowLevel(\_:) 

Instance Method

# windowLevel(\_:)

Sets the window level of this scene.

macOS 15.0+

``` source
nonisolated
func windowLevel(_ level: WindowLevel) -> some Scene
```

## Parameters 

`level`  

The desired window level

## Discussion

```
Window("Utility Window", id: "...") {
    UtilityContent()
}
.windowLevel(.floating)
```

## See Also

### Positioning a window

func defaultPosition(UnitPoint) -> some Scene

Sets a default position for a window.

struct WindowLevel

The level of a window.

struct WindowLayoutRoot

A proxy which represents the root contents of a window.

struct WindowPlacement

A type which represents a preferred size and position for a window.

func defaultWindowPlacement((WindowLayoutRoot, WindowPlacementContext) -> WindowPlacement) -> some Scene

Defines a function used for determining the default placement of windows.

func windowIdealPlacement((WindowLayoutRoot, WindowPlacementContext) -> WindowPlacement) -> some Scene

Provides a function which determines a placement to use when windows of a scene zoom.

struct WindowPlacementContext

A type which represents contextual information used for sizing and positioning windows.

struct WindowProxy

The proxy for an open window in the app.

struct DisplayProxy

A type which provides information about display hardware.

