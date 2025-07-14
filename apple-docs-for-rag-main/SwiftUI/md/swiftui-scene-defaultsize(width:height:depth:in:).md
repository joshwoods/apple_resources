

- SwiftUI
- Scene
-  defaultSize(width:height:depth:in:) 

Instance Method

# defaultSize(width:height:depth:in:)

Sets a default size for a volumetric window.

visionOS 1.0+

``` source
nonisolated
func defaultSize(
    width: CGFloat,
    height: CGFloat,
    depth: CGFloat,
    in unit: UnitLength
) -> some Scene
```

## Parameters 

`width`  

The default width for the created window.

`height`  

The default height for the created window.

`depth`  

The default depth for the created volumetric window.

`unit`  

The unit of length the dimensions of the window are specified in.

## Return Value

A scene that uses a default size for new windows.

## Discussion

Use this modifier to indicate the default initial size for a new 3D window created from a Scene using VolumetricWindowStyle:

```
WindowGroup {
    ContentView()
}
.windowStyle(.volumetric)
.defaultSize(width: 1, height: 1, depth: 0.5, in: .meters)
```

Each parameter is specified in the unit you provide. The size of a volumetric scene is immutable after creation.

This modifier affects only windows that have the volumetric style in visionOS.

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

func windowResizability(WindowResizability) -> some Scene

Sets the kind of resizability to use for a window.

struct WindowResizability

The resizability of a window.

func windowIdealSize(WindowIdealSize) -> some Scene

Specifies how windows derived form this scene should determine their size when zooming.

struct WindowIdealSize

A type which defines the size a window should use when zooming.

