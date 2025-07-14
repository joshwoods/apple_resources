

- SwiftUI
- Scene
-  windowResizability(\_:) 

Instance Method

# windowResizability(\_:)

Sets the kind of resizability to use for a window.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
nonisolated
func windowResizability(_ resizability: WindowResizability) -> some Scene
```

## Parameters 

`resizability`  

The resizability to use for windows created by this scene.

## Return Value

A scene that uses the specified resizability strategy.

## Discussion

Use this scene modifier to apply a value of type WindowResizability to a Scene that you define in your App declaration. The value that you specify indicates the strategy the system uses to place minimum and maximum size restrictions on windows that it creates from that scene.

For example, you can create a window group that people can resize to between 100 and 400 points in both dimensions by applying both a frame with those constraints to the scene’s content, and the contentSize resizability to the scene:

```
@main
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
                .frame(
                    minWidth: 100, maxWidth: 400,
                    minHeight: 100, maxHeight: 400)
        }
        .windowResizability(.contentSize)
    }
}
```

The default value for all scenes if you don’t apply the modifier is automatic. With that strategy, Settings windows use the contentSize strategy, while all others use contentMinSize.

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

struct WindowResizability

The resizability of a window.

func windowIdealSize(WindowIdealSize) -> some Scene

Specifies how windows derived form this scene should determine their size when zooming.

struct WindowIdealSize

A type which defines the size a window should use when zooming.

