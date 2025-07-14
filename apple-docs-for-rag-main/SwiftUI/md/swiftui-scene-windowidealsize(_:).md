

- SwiftUI
- Scene
-  windowIdealSize(\_:) 

Instance Method

# windowIdealSize(\_:)

Specifies how windows derived form this scene should determine their size when zooming.

macOS 15.0+

``` source
nonisolated
func windowIdealSize(_ idealSize: WindowIdealSize) -> some Scene
```

## Parameters 

`idealSize`  

A value which determines how windows derived from this scene should size themselves when zooming.

## Discussion

The default behavior will size the window to its maximum size, or the bounds of the display, whichever is smaller. By overriding this behavior, you can provide a size that is appropriate for the contents of your window.

For example, you can define a window group where the window has an ideal width of 800 points and an ideal height of 600 points:

```
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
                .frame(idealWidth: 800, idealHeight: 600)
        }
        .windowIdealSize(.fitToContent)
    }
}
```

## See Also

### Sizing a window

Positioning and sizing windows

Influence the initial geometry of windows that your app presents.

func defaultSize(_:)

Sets a default size for a window.

func defaultSize(width: CGFloat, height: CGFloat) -> some Scene

Sets a default width and height for a window.

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

struct WindowIdealSize

A type which defines the size a window should use when zooming.

