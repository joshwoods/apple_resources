

- SwiftUI
-  WindowProxy 

Structure

# WindowProxy

The proxy for an open window in the app.

visionOS 2.0+

``` source
struct WindowProxy
```

## Topics

### Instance Properties

var id: String?

The ID for the window, if one was provided.

var phase: ScenePhase

The window’s current ScenePhase.

## See Also

### Positioning a window

func defaultPosition(UnitPoint) -> some Scene

Sets a default position for a window.

struct WindowLevel

The level of a window.

func windowLevel(WindowLevel) -> some Scene

Sets the window level of this scene.

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

struct DisplayProxy

A type which provides information about display hardware.

