

- SwiftUI
- View
-  backgroundStyle(\_:) 

Instance Method

# backgroundStyle(\_:)

Sets the specified style to render backgrounds within the view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func backgroundStyle(_ style: S) -> some View where S : ShapeStyle
```

## Discussion

The following example uses this modifier to set the backgroundStyle environment value to a blue color that includes a subtle gradient. SwiftUI fills the Circle shape that acts as a background element with this style:

```
Image(systemName: "swift")
    .padding()
    .background(in: Circle())
    .backgroundStyle(.blue.gradient)
```

To restore the default background style, set the backgroundStyle environment value to `nil` using the environment(_:_:) modifer:

```
.environment(\.backgroundStyle, nil)
```

## See Also

### Styling content

func border&lt;S>(S, width: CGFloat) -> some View

Adds a border to this view with the specified style and width.

func foregroundStyle&lt;S>(S) -> some View

Sets a view’s foreground elements to use a given style.

func foregroundStyle&lt;S1, S2>(S1, S2) -> some View

Sets the primary and secondary levels of the foreground style in the child view.

func foregroundStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the primary, secondary, and tertiary levels of the foreground style.

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

