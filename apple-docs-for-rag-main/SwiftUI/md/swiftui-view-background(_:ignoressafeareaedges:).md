

- SwiftUI
- View
-  background(\_:ignoresSafeAreaEdges:) 

Instance Method

# background(\_:ignoresSafeAreaEdges:)

Sets the view’s background to a style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func background(
    _ style: S,
    ignoresSafeAreaEdges edges: Edge.Set = .all
) -> some View where S : ShapeStyle
```

## Parameters 

`style`  

An instance of a type that conforms to ShapeStyle that SwiftUI draws behind the modified view.

`edges`  

The set of edges for which to ignore safe area insets when adding the background. The default value is all. Specify an empty set to respect safe area insets on all edges.

## Return Value

A view with the specified style drawn behind it.

## Discussion

Use this modifier to place a type that conforms to the ShapeStyle protocol — like a Color, Material, or HierarchicalShapeStyle — behind a view. For example, you can add the regularMaterial behind a Label:

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

SwiftUI limits the background style’s extent to the modified view’s container-relative shape. You can see this effect if you constrain the `FlagLabel` view with a containerShape(_:) modifier:

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

If you want to specify a View or a stack of views as the background, use background(alignment:content:) instead. To specify a Shape or InsettableShape, use background(_:in:fillStyle:) . To configure the background of a presentation, like a sheet, use presentationBackground(_:).

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

