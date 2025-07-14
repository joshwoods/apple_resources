

- Symbols
- VariableColorSymbolEffect
-  iterative 

Instance Property

# iterative

An effect that momentarily enables each layer of a symbol-based image in sequence.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var iterative: VariableColorSymbolEffect { get }
```

## Discussion

This effect enables each successive variable layer for a short period of time, and then disables the layer until the animation cycle ends. This effect cancels the cumulative variant.

## See Also

### Controlling fill style

var cumulative: VariableColorSymbolEffect

An effect that enables each layer of a symbol-based image in sequence.

