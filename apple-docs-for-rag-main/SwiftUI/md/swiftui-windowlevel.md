

- SwiftUI
-  WindowLevel 

Structure

# WindowLevel

The level of a window.

macOS 15.0+

``` source
struct WindowLevel
```

## Overview

Use this in conjunction with the `.windowLevel(_:)` modifier to control window levels.

## Topics

### Type Properties

static var automatic: WindowLevel

Automatic window level.

static var desktop: WindowLevel

Desktop window level.

static var floating: WindowLevel

Floating window level.

static var normal: WindowLevel

Normal window level.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Positioning a window

func defaultPosition(UnitPoint) -> some Scene

Sets a default position for a window.

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

struct WindowProxy

The proxy for an open window in the app.

struct DisplayProxy

A type which provides information about display hardware.

