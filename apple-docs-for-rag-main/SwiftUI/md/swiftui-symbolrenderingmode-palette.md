

- SwiftUI
- SymbolRenderingMode
-  palette 

Type Property

# palette

A mode that renders symbols as multiple layers, with different styles applied to the layers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let palette: SymbolRenderingMode
```

## Discussion

In this mode SwiftUI maps each successively defined layer in the image to the next of the primary, secondary, and tertiary variants of the foreground style. You can specify these styles explicitly using the foregroundStyle(_:_:) and foregroundStyle(_:_:_:) modifiers. If you only specify a primary foreground style, SwiftUI automatically derives the others from that style. For example, you can render a filled exclamation mark triangle with yellow as the tint color for the exclamation mark, and fill the triangle with cyan:

```
Image(systemName: "exclamationmark.triangle.fill")
    .symbolRenderingMode(.palette)
    .foregroundStyle(Color.yellow, Color.cyan)
```

You can also omit the symbol rendering mode, as specifying multiple foreground styles implies switching to palette rendering mode:

```
Image(systemName: "exclamationmark.triangle.fill")
    .foregroundStyle(Color.yellow, Color.cyan)
```

## See Also

### Getting symbol rendering modes

static let hierarchical: SymbolRenderingMode

A mode that renders symbols as multiple layers, with different opacities applied to the foreground style.

static let monochrome: SymbolRenderingMode

A mode that renders symbols as a single layer filled with the foreground style.

static let multicolor: SymbolRenderingMode

A mode that renders symbols as multiple layers with their inherit styles.

