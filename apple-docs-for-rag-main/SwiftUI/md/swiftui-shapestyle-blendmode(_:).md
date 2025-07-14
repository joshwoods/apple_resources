

- SwiftUI
- ShapeStyle
-  blendMode(\_:) 

Type Method

# blendMode(\_:)

Returns a new style based on the current style that uses `mode` as its blend mode when drawing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func blendMode(_ mode: BlendMode) -> some ShapeStyle
```

Available when `Self` is `AnyShapeStyle`.

## Discussion

In most contexts the current style is the foreground but e.g. when setting the value of the background style, that becomes the current implicit style.

For example, a circle filled with the current foreground style and the overlay blend mode:

```
Circle().fill(.blendMode(.overlay))
```

## See Also

### Configuring the default shape style

static func opacity(Double) -> some ShapeStyle

Returns a new style based on the current style that multiplies by `opacity` when drawing.

static func shadow(ShadowStyle) -> some ShapeStyle

Returns a shape style that applies the specified shadow style to the current style.

