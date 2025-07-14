

- SwiftUI
- SymbolRenderingMode
-  multicolor 

Type Property

# multicolor

A mode that renders symbols as multiple layers with their inherit styles.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let multicolor: SymbolRenderingMode
```

## Discussion

The layers may be filled with their own inherent styles, or the foreground style. For example, you can render a filled exclamation mark triangle in its inherent colors, with yellow for the triangle and white for the exclamation mark:

```
Image(systemName: "exclamationmark.triangle.fill")
    .symbolRenderingMode(.multicolor)
```

## See Also

### Getting symbol rendering modes

static let hierarchical: SymbolRenderingMode

A mode that renders symbols as multiple layers, with different opacities applied to the foreground style.

static let monochrome: SymbolRenderingMode

A mode that renders symbols as a single layer filled with the foreground style.

static let palette: SymbolRenderingMode

A mode that renders symbols as multiple layers, with different styles applied to the layers.

