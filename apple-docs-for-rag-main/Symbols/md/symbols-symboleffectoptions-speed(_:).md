

- Symbols
- SymbolEffectOptions
-  speed(\_:) 

Type Method

# speed(\_:)

A default set of effect options with a preferred speed multiplier.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func speed(_ speed: Double) -> SymbolEffectOptions
```

## Parameters 

`speed`  

The preferred speed multiplier to play the effect with. The default multiplier is `1.0`. The function may clamp very large or small values.

## Return Value

A new set of effect options with the preferred speed multiplier.

## See Also

### Configuring effect speed

func speed(Double) -> SymbolEffectOptions

Creates a set of effect options with a preferred speed multiplier.

