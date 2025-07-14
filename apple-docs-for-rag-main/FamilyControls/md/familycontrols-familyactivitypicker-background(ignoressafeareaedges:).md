

- FamilyControls
- FamilyActivityPicker
-  background(ignoresSafeAreaEdges:) 

Instance Method

# background(ignoresSafeAreaEdges:)

Sets the view’s background to the default background style.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func background(ignoresSafeAreaEdges edges: Edge.Set = .all) -> some View
```

## Parameters 

`edges`  

The set of edges for which to ignore safe area insets when adding the background. The default value is `Edge/Set/all`. Specify an empty set to respect safe area insets on all edges.

## Return Value

A view with the `ShapeStyle/background` shape style drawn behind it.

## Discussion

This modifier behaves like `View/background(_:ignoresSafeAreaEdges:)`, except that it always uses the `ShapeStyle/background` shape style. For example, you can add a background to a `Label`:

```
ZStack {
    Color.teal
    Label("Flag", systemImage: "flag.fill")
        .padding()
        .background()
}
```

Without the background modifier, the teal color behind the label shows through the label. With the modifier, the label’s text and icon appear backed by a region filled with a color that’s appropriate for light or dark appearance:

If you want to specify a `View` or a stack of views as the background, use `View/background(alignment:content:)` instead. To specify a `Shape` or `InsettableShape`, use `View/background(_:in:fillStyle:)`. To configure the background of a presentation, like a sheet, use `View/presentationBackground(_:)`.

## See Also

### Background Elements

func border&lt;S>(S, width: CGFloat) -> some View

Adds a border to this view with the specified style and width.

func background&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to a style.

func background&lt;S>(in: S, fillStyle: FillStyle) -> some View

Sets the view’s background to a shape filled with the default background style.

func background&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Sets the view’s background to a shape filled with a style.

func background&lt;S>(in: S, fillStyle: FillStyle) -> some View

Sets the view’s background to an insettable shape filled with the default background style.

func background&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Sets the view’s background to an insettable shape filled with a style.

func listRowBackground&lt;V>(V?) -> some View

Places a custom background view behind a list row item.

