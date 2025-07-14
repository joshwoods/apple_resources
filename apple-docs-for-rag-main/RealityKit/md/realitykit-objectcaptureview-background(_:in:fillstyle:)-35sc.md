

- RealityKit
- ObjectCaptureView
-  background(\_:in:fillStyle:) 

Instance Method

# background(\_:in:fillStyle:)

Sets the view’s background to a shape filled with a style.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func background(
    _ style: S,
    in shape: T,
    fillStyle: FillStyle = FillStyle()
) -> some View where S : ShapeStyle, T : Shape
```

## Parameters 

`style`  

A `ShapeStyle` that SwiftUI uses to the fill the shape that you specify.

`shape`  

An instance of a type that conforms to `Shape` that SwiftUI draws behind the view.

`fillStyle`  

The `FillStyle` to use when drawing the shape. The default style uses the nonzero winding number rule and antialiasing.

## Return Value

A view with the specified shape drawn behind it.

## Discussion

Use this modifier to layer a type that conforms to the `Shape` protocol behind a view. Specify the `ShapeStyle` that’s used to fill the shape. For example, you can create a `Path` that outlines a trapezoid:

```
let trapezoid = Path { path in
    path.move(to: .zero)
    path.addLine(to: CGPoint(x: 90, y: 0))
    path.addLine(to: CGPoint(x: 80, y: 50))
    path.addLine(to: CGPoint(x: 10, y: 50))
}
```

Then you can use that shape as a background for a `Label`:

```
Label("Flag", systemImage: "flag.fill")
    .padding()
    .background(.teal, in: trapezoid)
```

The `ShapeStyle/teal` color fills the shape:

This modifier is a convenience method for placing a single shape behind a view. To create a background with other `View` types — or with a stack of views — use `View/background(alignment:content:)` instead. To add a `ShapeStyle` as a background, use `View/background(_:ignoresSafeAreaEdges:)`.

