

- SwiftUI
- View
-  background(\_:in:fillStyle:) 

Instance Method

# background(\_:in:fillStyle:)

Sets the view’s background to an insettable shape filled with a style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func background(
    _ style: S,
    in shape: T,
    fillStyle: FillStyle = FillStyle()
) -> some View where S : ShapeStyle, T : InsettableShape
```

Show all declarations

## Parameters 

`style`  

A ShapeStyle that SwiftUI uses to the fill the shape that you specify.

`shape`  

An instance of a type that conforms to InsettableShape that SwiftUI draws behind the view.

`fillStyle`  

The FillStyle to use when drawing the shape. The default style uses the nonzero winding number rule and antialiasing.

## Return Value

A view with the specified insettable shape drawn behind it.

## Discussion

Use this modifier to layer a type that conforms to the InsettableShape protocol — like a Rectangle, Circle, or Capsule — behind a view. Specify the ShapeStyle that’s used to fill the shape. For example, you can place a RoundedRectangle behind a Label:

```
Label("Flag", systemImage: "flag.fill")
    .padding()
    .background(.teal, in: RoundedRectangle(cornerRadius: 8))
```

The teal color fills the shape:

This modifier is a convenience method for placing a single shape behind a view. To create a background with other View types — or with a stack of views — use background(alignment:content:) instead. To add a ShapeStyle as a background, use background(_:ignoresSafeAreaEdges:).

## See Also

### Layering views

Adding a background to your view

Compose a background behind your view and extend it beyond the safe area insets.

struct ZStack

A view that overlays its subviews, aligning them in both axes.

func zIndex(Double) -> some View

Controls the display order of overlapping views.

func background&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify behind this view.

func background&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to a style.

func background(ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to the default background style.

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

