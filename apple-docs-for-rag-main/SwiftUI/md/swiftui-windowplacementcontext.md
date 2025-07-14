

- SwiftUI
-  WindowPlacementContext 

Structure

# WindowPlacementContext

A type which represents contextual information used for sizing and positioning windows.

macOS 15.0+visionOS 2.0+

``` source
struct WindowPlacementContext
```

## Overview

The placement context provides information to be used when providing a new placement via the closure provided to the `defaultWindowPlacement(_:)` modifier.

## Topics

### Instance Properties

var defaultDisplay: DisplayProxy

The display on which new windows will be presented by default.

var windows: [WindowProxy]

The list of current active scenes

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

struct WindowProxy

The proxy for an open window in the app.

struct DisplayProxy

A type which provides information about display hardware.

