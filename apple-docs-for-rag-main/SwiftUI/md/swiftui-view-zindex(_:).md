

- SwiftUI
- View
-  zIndex(\_:) 

Instance Method

# zIndex(\_:)

Controls the display order of overlapping views.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func zIndex(_ value: Double) -> some View
```

## Parameters 

`value`  

A relative front-to-back ordering for this view; the default is `0`.

## Discussion

Use `zIndex(_:)` when you want to control the front-to-back ordering of views.

In this example there are two overlapping rotated rectangles. The frontmost is represented by the larger index value.

```
VStack {
    Rectangle()
        .fill(Color.yellow)
        .frame(width: 100, height: 100, alignment: .center)
        .zIndex(1) // Top layer.

    Rectangle()
        .fill(Color.red)
        .frame(width: 100, height: 100, alignment: .center)
        .rotationEffect(.degrees(45))
        // Here a zIndex of 0 is the default making
        // this the bottom layer.
}
```

## See Also

### Layering views

Adding a background to your view

Compose a background behind your view and extend it beyond the safe area insets.

struct ZStack

A view that overlays its subviews, aligning them in both axes.

func background&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify behind this view.

func background&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to a style.

func background(ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to the default background style.

func background(_:in:fillStyle:)

Sets the view’s background to an insettable shape filled with a style.

func background(in:fillStyle:)

Sets the view’s background to an insettable shape filled with the default background style.

func overlay&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify in front of this view.

func overlay&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Layers the specified style in front of this view.

func overlay&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Layers a shape that you specify in front of this view.

var backgroundMaterial: Material?

The material underneath the current view.

func containerBackground&lt;S>(S, for: ContainerBackgroundPlacement) -> some View

Sets the container background of the enclosing container using a view.

func containerBackground&lt;V>(for: ContainerBackgroundPlacement, alignment: Alignment, content: () -> V) -> some View

Sets the container background of the enclosing container using a view.

struct ContainerBackgroundPlacement

The placement of a container background.

