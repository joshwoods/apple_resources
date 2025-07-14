

- SwiftUI
- Scene
-  defaultSize(width:height:) 

Instance Method

# defaultSize(width:height:)

Sets a default width and height for a window.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
nonisolated
func defaultSize(
    width: CGFloat,
    height: CGFloat
) -> some Scene
```

## Parameters 

`width`  

The default width for windows created from a scene.

`height`  

The default height for windows created from a scene.

## Return Value

A scene that uses a default size for new windows.

## Discussion

Use this scene modifier to indicate a default initial size for a new window that the system creates from a Scene declaration. For example, you can request that new windows that a WindowGroup generates occupy 600 points in the x-dimension and 400 points in the y-dimension:

```
@main
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
        .defaultSize(width: 600, height: 400)
    }
}
```

The size that you specify acts only as a default for when the window first appears. People can later resize the window using interface controls that the system provides. Also, during state restoration, the system restores windows to their most recent size rather than the default size.

If you specify a default size that’s outside the range of the window’s inherent resizability in one or both dimensions, the system clamps the affected dimension to keep it in range. You can configure the resizability of a scene using the windowResizability(_:) modifier.

The default size modifier affects any scene type that creates windows in macOS, namely:

- WindowGroup

- Window

- DocumentGroup

- Settings

If you want to specify the size input in terms of size instance, use defaultSize(_:) instead.

## See Also

### Sizing a window

Positioning and sizing windows

Influence the initial geometry of windows that your app presents.

func defaultSize(_:)

Sets a default size for a window.

func defaultSize(width: CGFloat, height: CGFloat, depth: CGFloat) -> some Scene

Sets a default size for a volumetric window.

func defaultSize(Size3D, in: UnitLength) -> some Scene

Sets a default size for a volumetric window.

func defaultSize(width: CGFloat, height: CGFloat, depth: CGFloat, in: UnitLength) -> some Scene

Sets a default size for a volumetric window.

func windowResizability(WindowResizability) -> some Scene

Sets the kind of resizability to use for a window.

struct WindowResizability

The resizability of a window.

func windowIdealSize(WindowIdealSize) -> some Scene

Specifies how windows derived form this scene should determine their size when zooming.

struct WindowIdealSize

A type which defines the size a window should use when zooming.

