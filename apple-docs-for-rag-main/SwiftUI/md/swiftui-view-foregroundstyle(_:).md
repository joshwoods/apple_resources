

- SwiftUI
- View
-  foregroundStyle(\_:) 

Instance Method

# foregroundStyle(\_:)

Sets a view’s foreground elements to use a given style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func foregroundStyle(_ style: S) -> some View where S : ShapeStyle
```

## Parameters 

`style`  

The color or pattern to use when filling in the foreground elements. To indicate a specific value, use Color or image(_:sourceRect:scale:), or one of the gradient types, like linearGradient(colors:startPoint:endPoint:). To set a style that’s relative to the containing view’s style, use one of the semantic styles, like primary.

## Return Value

A view that uses the given foreground style.

## Discussion

Use this method to style foreground content like text, shapes, and template images (including symbols):

```
HStack {
    Image(systemName: "triangle.fill")
    Text("Hello, world!")
    RoundedRectangle(cornerRadius: 5)
        .frame(width: 40, height: 20)
}
.foregroundStyle(.teal)
```

The example above creates a row of teal foreground elements:

You can use any style that conforms to the ShapeStyle protocol, like the teal color in the example above, or the linearGradient(colors:startPoint:endPoint:) gradient shown below:

```
Text("Gradient Text")
    .font(.largeTitle)
    .foregroundStyle(
        .linearGradient(
            colors: [.yellow, .blue],
            startPoint: .top,
            endPoint: .bottom
        )
    )
```

Tip

If you want to fill a single Shape instance with a style, use the fill(style:) shape modifier instead because it’s more efficient.

SwiftUI creates a context-dependent render for a given style. For example, a Color that you load from an asset catalog can have different light and dark appearances, while some styles also vary by platform.

Hierarchical foreground styles like `ShapeStyle/secondary` don’t impose a style of their own, but instead modify other styles. In particular, they modify the primary level of the current foreground style to the degree given by the hierarchical style’s name. To find the current foreground style to modify, SwiftUI looks for the innermost containing style that you apply with the `foregroundStyle(_:)` or the foregroundColor(_:) modifier. If you haven’t specified a style, SwiftUI uses the default foreground style, as in the following example:

```
VStack(alignment: .leading) {
    Label("Primary", systemImage: "1.square.fill")
    Label("Secondary", systemImage: "2.square.fill")
        .foregroundStyle(.secondary)
}
```

If you add a foreground style on the enclosing VStack, the hierarchical styling responds accordingly:

```
VStack(alignment: .leading) {
    Label("Primary", systemImage: "1.square.fill")
    Label("Secondary", systemImage: "2.square.fill")
        .foregroundStyle(.secondary)
}
.foregroundStyle(.blue)
```

When you apply a custom style to a view, the view disables the vibrancy effect for foreground elements in that view, or in any of its child views, that it would otherwise gain from adding a background material — for example, using the background(_:ignoresSafeAreaEdges:) modifier. However, hierarchical styles applied to the default foreground don’t disable vibrancy.

## See Also

### Styling content

func border&lt;S>(S, width: CGFloat) -> some View

Adds a border to this view with the specified style and width.

func foregroundStyle&lt;S1, S2>(S1, S2) -> some View

Sets the primary and secondary levels of the foreground style in the child view.

func foregroundStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the primary, secondary, and tertiary levels of the foreground style.

func backgroundStyle&lt;S>(S) -> some View

Sets the specified style to render backgrounds within the view.

var backgroundStyle: AnyShapeStyle?

An optional style that overrides the default system background style when set.

protocol ShapeStyle

A color or pattern to use when rendering a shape.

struct AnyShapeStyle

A type-erased ShapeStyle value.

struct Gradient

A color gradient represented as an array of color stops, each having a parametric location value.

struct MeshGradient

A two-dimensional gradient defined by a 2D grid of positioned colors.

struct AnyGradient

A color gradient.

struct ShadowStyle

A style to use when rendering shadows.

