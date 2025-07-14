

- SwiftUI
-  WindowLayoutRoot 

Structure

# WindowLayoutRoot

A proxy which represents the root contents of a window.

macOS 15.0+visionOS 2.0+

``` source
struct WindowLayoutRoot
```

## Overview

This type acts like a proxy for the contents of the window defined by a SwiftUI Scene. The `Scene.defaultWindowPlacement(_:)` modifier receives an instance of this type, representing the contents of the window being created.

Use this proxy to get information about the window’s contents, like it’s size.

## Topics

### Instance Methods

func sizeThatFits(ProposedViewSize) -> CGSize

Asks the window’s content for its size.

## See Also

### Positioning a window

func defaultPosition(UnitPoint) -> some Scene

Sets a default position for a window.

struct WindowLevel

The level of a window.

func windowLevel(WindowLevel) -> some Scene

Sets the window level of this scene.

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

