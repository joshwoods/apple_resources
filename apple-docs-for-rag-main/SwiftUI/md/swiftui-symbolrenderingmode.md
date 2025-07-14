

- SwiftUI
-  SymbolRenderingMode 

Structure

# SymbolRenderingMode

A symbol rendering mode.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SymbolRenderingMode
```

## Topics

### Getting symbol rendering modes

static let hierarchical: SymbolRenderingMode

A mode that renders symbols as multiple layers, with different opacities applied to the foreground style.

static let monochrome: SymbolRenderingMode

A mode that renders symbols as a single layer filled with the foreground style.

static let multicolor: SymbolRenderingMode

A mode that renders symbols as multiple layers with their inherit styles.

static let palette: SymbolRenderingMode

A mode that renders symbols as multiple layers, with different styles applied to the layers.

## Relationships

### Conforms To

- Sendable

## See Also

### Setting symbol rendering modes

func symbolRenderingMode(SymbolRenderingMode?) -> some View

Sets the rendering mode for symbol images within this view.

var symbolRenderingMode: SymbolRenderingMode?

The current symbol rendering mode, or `nil` denoting that the mode is picked automatically using the current image and foreground style as parameters.

