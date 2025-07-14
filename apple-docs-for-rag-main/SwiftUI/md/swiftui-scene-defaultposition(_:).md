

- SwiftUI
- Scene
-  defaultPosition(\_:) 

Instance Method

# defaultPosition(\_:)

Sets a default position for a window.

macOS 13.0+

``` source
nonisolated
func defaultPosition(_ position: UnitPoint) -> some Scene
```

## Parameters 

`position`  

A UnitPoint that specifies where to place a newly opened window relative to the screen bounds.

## Return Value

A scene that uses a default position for new windows.

## Discussion

The first time your app opens a window from a particular scene declaration, the system places the window at the center of the screen by default. For scene types that support multiple simultaneous windows, the system offsets each additional window by a small amount to avoid completely obscuring existing windows.

You can override the default placement of the first window by applying a scene modifier that indicates where to place the window relative to the screen bounds. For example, you can request that the system place a new window in the bottom trailing corner of the screen:

```
@main
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
        .defaultPosition(.bottomTrailing)
    }
}
```

The system aligns the point in the window that corresponds to the specified UnitPoint with the point in the screen that corresponds to the same unit point.

You typically use one of the predefined unit points — like bottomTrailing in the above example — but you can also use a custom unit point. For example, the following modifier aligns the point that’s one quarter of the way from the leading edge of the window with the point that’s one quarter of the way from the leading edge of the screen, while centering the window in the y-dimension:

```
WindowGroup {
    ContentView()
}
.defaultPosition(UnitPoint(x: 0.25, y: 0.5))
```

The modifier affects any scene type that creates windows in macOS, namely:

- WindowGroup

- Window

- DocumentGroup

- Settings

The value that you provide acts only as an initial default. During state restoration, the system restores the window to the position that it last occupied.

## See Also

### Positioning a window

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

struct DisplayProxy

A type which provides information about display hardware.

