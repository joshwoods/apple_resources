

- SwiftUI
- SymbolRenderingMode
-  hierarchical 

Type Property

# hierarchical

A mode that renders symbols as multiple layers, with different opacities applied to the foreground style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let hierarchical: SymbolRenderingMode
```

## Discussion

SwiftUI fills the first layer with the foreground style, and the others the secondary, and tertiary variants of the foreground style. You can specify these styles explicitly using the foregroundStyle(_:_:) and foregroundStyle(_:_:_:) modifiers. If you only specify a primary foreground style, SwiftUI automatically derives the others from that style. For example, you can render a filled exclamation mark triangle with purple as the tint color for the exclamation mark, and lower opacity purple for the triangle:

```
Image(systemName: "exclamationmark.triangle.fill")
    .symbolRenderingMode(.hierarchical)
    .foregroundStyle(Color.purple)
```

## See Also

### Getting symbol rendering modes

static let monochrome: SymbolRenderingMode

A mode that renders symbols as a single layer filled with the foreground style.

static let multicolor: SymbolRenderingMode

A mode that renders symbols as multiple layers with their inherit styles.

static let palette: SymbolRenderingMode

A mode that renders symbols as multiple layers, with different styles applied to the layers.

