

- Symbols
- VariableColorSymbolEffect
-  cumulative 

Instance Property

# cumulative

An effect that enables each layer of a symbol-based image in sequence.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var cumulative: VariableColorSymbolEffect { get }
```

## Discussion

This effect enables each successive variable layer, and the layer remains enabled until the end of the animation cycle. This effect cancels the iterative variant.

## See Also

### Controlling fill style

var iterative: VariableColorSymbolEffect

An effect that momentarily enables each layer of a symbol-based image in sequence.

