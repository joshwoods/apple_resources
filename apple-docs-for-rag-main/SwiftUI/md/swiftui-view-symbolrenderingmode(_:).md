

- SwiftUI
- View
-  symbolRenderingMode(\_:) 

Instance Method

# symbolRenderingMode(\_:)

Sets the rendering mode for symbol images within this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func symbolRenderingMode(_ mode: SymbolRenderingMode?) -> some View
```

## Parameters 

`mode`  

The symbol rendering mode to use.

## Return Value

A view that uses the rendering mode you supply.

## See Also

### Setting symbol rendering modes

var symbolRenderingMode: SymbolRenderingMode?

The current symbol rendering mode, or `nil` denoting that the mode is picked automatically using the current image and foreground style as parameters.

struct SymbolRenderingMode

A symbol rendering mode.

