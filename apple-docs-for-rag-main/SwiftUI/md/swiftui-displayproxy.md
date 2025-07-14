

- SwiftUI
-  DisplayProxy 

Structure

# DisplayProxy

A type which provides information about display hardware.

macOS 15.0+

``` source
struct DisplayProxy
```

## Overview

You can use this type with your custom window layouts to size and position windows relative to a display’s bounds.

For example, your custom window layout can position a window 140 points from the bottom of the screen’s visible area:

```
Window("Status", id: "status") {
    StatusView()
}
.windowResizability(.contentSize)
.defaultWindowPlacement { content, context in
    let displayBounds = context.defaultDisplay.visibleRect
    let size = content.sizeThatFits(.unspecified)
    let position = CGPoint(
        x: displayBounds.midX - (size.width / 2),
        y: displayBounds.maxY - size.height - 140)
    return WindowPlacement(position: position, size: size)
}
```

## Topics

### Instance Properties

let bounds: CGRect

The full dimensions of the display, including any space occupied by system interface elements.

let safeAreaInsets: EdgeInsets

The safe area inset of this display.

let visibleRect: CGRect

The portion of the display where it is safe to place windows.

## Relationships

### Conforms To

- Equatable

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

struct WindowProxy

The proxy for an open window in the app.

