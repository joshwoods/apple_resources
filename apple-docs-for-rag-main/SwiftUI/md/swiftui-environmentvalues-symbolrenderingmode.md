

- SwiftUI
- EnvironmentValues
-  symbolRenderingMode 

Instance Property

# symbolRenderingMode

The current symbol rendering mode, or `nil` denoting that the mode is picked automatically using the current image and foreground style as parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var symbolRenderingMode: SymbolRenderingMode? { get set }
```

## See Also

### Setting symbol rendering modes

func symbolRenderingMode(SymbolRenderingMode?) -> some View

Sets the rendering mode for symbol images within this view.

struct SymbolRenderingMode

A symbol rendering mode.

