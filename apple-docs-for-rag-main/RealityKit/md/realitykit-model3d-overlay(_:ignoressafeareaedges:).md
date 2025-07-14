

- RealityKit
- Model3D
-  overlay(\_:ignoresSafeAreaEdges:) 

Instance Method

# overlay(\_:ignoresSafeAreaEdges:)

Layers the specified style in front of this view.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func overlay(
    _ style: S,
    ignoresSafeAreaEdges edges: Edge.Set = .all
) -> some View where S : ShapeStyle
```

## Parameters 

`style`  

An instance of a type that conforms to `ShapeStyle` that SwiftUI layers in front of the modified view.

`edges`  

The set of edges for which to ignore safe area insets when adding the overlay. The default value is `Edge/Set/all`. Specify an empty set to respect safe area insets on all edges.

## Return Value

A view with the specified style drawn in front of it.

## Discussion

Use this modifier to layer a type that conforms to the `ShapeStyle` protocol, like a `Color`, Material, or `HierarchicalShapeStyle`, in front of a view. For example, you can overlay the `ShapeStyle/ultraThinMaterial` over a `Circle`:

```
struct CoveredCircle: View {
    var body: some View {
        Circle()
            .frame(width: 300, height: 200)
            .overlay(.ultraThinMaterial)
    }
}
```

SwiftUI anchors the style to the view’s bounds. For the example above, the overlay fills the entirety of the circle’s frame (which happens to be wider than the circle is tall):

SwiftUI also limits the style’s extent to the view’s container-relative shape. You can see this effect if you constrain the `CoveredCircle` view with a `View/containerShape(_:)` modifier:

```
CoveredCircle()
    .containerShape(RoundedRectangle(cornerRadius: 30))
```

The overlay takes on the specified container shape:

By default, the overlay ignores safe area insets on all edges, but you can provide a specific set of edges to ignore, or an empty set to respect safe area insets on all edges:

```
Rectangle()
    .overlay(
        .secondary,
        ignoresSafeAreaEdges: []) // Ignore no safe area insets.
```

If you want to specify a `View` or a stack of views as the overlay rather than a style, use `View/overlay(alignment:content:)` instead. If you want to specify a `Shape`, use `View/overlay(_:in:fillStyle:)`.

