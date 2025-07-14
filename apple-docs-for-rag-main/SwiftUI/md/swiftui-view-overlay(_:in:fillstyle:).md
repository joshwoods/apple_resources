

- SwiftUI
- View
-  overlay(\_:in:fillStyle:) 

Instance Method

# overlay(\_:in:fillStyle:)

Layers a shape that you specify in front of this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func overlay(
    _ style: S,
    in shape: T,
    fillStyle: FillStyle = FillStyle()
) -> some View where S : ShapeStyle, T : Shape
```

## Parameters 

`style`  

A ShapeStyle that SwiftUI uses to the fill the shape that you specify.

`shape`  

An instance of a type that conforms to Shape that SwiftUI draws in front of the view.

`fillStyle`  

The FillStyle to use when drawing the shape. The default style uses the nonzero winding number rule and antialiasing.

## Return Value

A view with the specified shape drawn in front of it.

## Discussion

Use this modifier to layer a type that conforms to the Shape protocol — like a Rectangle, Circle, or Capsule — in front of a view. Specify a ShapeStyle that’s used to fill the shape. For example, you can overlay the outline of one rectangle in front of another:

```
Rectangle()
    .frame(width: 200, height: 100)
    .overlay(.teal, in: Rectangle().inset(by: 10).stroke(lineWidth: 5))
```

The example above uses the inset(by:) method to slightly reduce the size of the overlaid rectangle, and the stroke(lineWidth:) method to fill only the shape’s outline. This creates an inset border:

This modifier is a convenience method for layering a shape over a view. To handle the more general case of overlaying a View — or a stack of views — with control over the position, use overlay(alignment:content:) instead. To cover a view with a ShapeStyle, use overlay(_:ignoresSafeAreaEdges:).

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

func background(_:in:fillStyle:)

Sets the view’s background to an insettable shape filled with a style.

func background(in:fillStyle:)

Sets the view’s background to an insettable shape filled with the default background style.

func overlay&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify in front of this view.

func overlay&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Layers the specified style in front of this view.

var backgroundMaterial: Material?

The material underneath the current view.

func containerBackground&lt;S>(S, for: ContainerBackgroundPlacement) -> some View

Sets the container background of the enclosing container using a view.

func containerBackground&lt;V>(for: ContainerBackgroundPlacement, alignment: Alignment, content: () -> V) -> some View

Sets the container background of the enclosing container using a view.

struct ContainerBackgroundPlacement

The placement of a container background.

