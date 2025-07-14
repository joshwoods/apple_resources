

- RealityKit
- RealityViewAttachmentBuilderContent
-  background(\_:ignoresSafeAreaEdges:) 

Instance Method

# background(\_:ignoresSafeAreaEdges:)

Sets the view’s background to a style.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func background(
    _ style: S,
    ignoresSafeAreaEdges edges: Edge.Set = .all
) -> some View where S : ShapeStyle
```

## Parameters 

`style`  

An instance of a type that conforms to `ShapeStyle` that SwiftUI draws behind the modified view.

`edges`  

The set of edges for which to ignore safe area insets when adding the background. The default value is `Edge/Set/all`. Specify an empty set to respect safe area insets on all edges.

## Return Value

A view with the specified style drawn behind it.

## Discussion

Use this modifier to place a type that conforms to the `ShapeStyle` protocol — like a `Color`, Material, or `HierarchicalShapeStyle` — behind a view. For example, you can add the `ShapeStyle/regularMaterial` behind a `Label`:

```
struct FlagLabel: View {
    var body: some View {
        Label("Flag", systemImage: "flag.fill")
            .padding()
            .background(.regularMaterial)
    }
}
```

SwiftUI anchors the style to the view’s bounds. For the example above, the background fills the entirety of the label’s frame, which includes the padding:

SwiftUI limits the background style’s extent to the modified view’s container-relative shape. You can see this effect if you constrain the `FlagLabel` view with a `View/containerShape(_:)` modifier:

```
FlagLabel()
    .containerShape(RoundedRectangle(cornerRadius: 16))
```

The background takes on the specified container shape:

By default, the background ignores safe area insets on all edges, but you can provide a specific set of edges to ignore, or an empty set to respect safe area insets on all edges:

```
Rectangle()
    .background(
        .regularMaterial,
        ignoresSafeAreaEdges: []) // Ignore no safe area insets.
```

If you want to specify a `View` or a stack of views as the background, use `View/background(alignment:content:)` instead. To specify a `Shape` or `InsettableShape`, use `View/background(_:in:fillStyle:)` . To configure the background of a presentation, like a sheet, use `View/presentationBackground(_:)`.

