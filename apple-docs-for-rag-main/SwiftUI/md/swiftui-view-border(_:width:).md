

- SwiftUI
- View
-  border(\_:width:) 

Instance Method

# border(\_:width:)

Adds a border to this view with the specified style and width.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func border(
    _ content: S,
    width: CGFloat = 1
) -> some View where S : ShapeStyle
```

## Parameters 

`content`  

A value that conforms to the ShapeStyle protocol, like a Color or HierarchicalShapeStyle, that SwiftUI uses to fill the border.

`width`  

The thickness of the border. The default is 1 pixel.

## Return Value

A view that adds a border with the specified style and width to this view.

## Mentioned in 

Configuring views

Inspecting view layout

## Discussion

Use this modifier to draw a border of a specified width around the view’s frame. By default, the border appears inside the bounds of this view. For example, you can add a four-point wide border covers the text:

```
Text("Purple border inside the view bounds.")
    .border(Color.purple, width: 4)
```

To place a border around the outside of this view, apply padding of the same width before adding the border:

```
Text("Purple border outside the view bounds.")
    .padding(4)
    .border(Color.purple, width: 4)
```

## See Also

### Styling content

func foregroundStyle&lt;S>(S) -> some View

Sets a view’s foreground elements to use a given style.

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

