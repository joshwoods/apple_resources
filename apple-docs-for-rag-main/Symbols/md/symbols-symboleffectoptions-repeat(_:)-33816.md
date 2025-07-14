

- Symbols
- SymbolEffectOptions
-  repeat(\_:) 

Type Method

# repeat(\_:)

A default set of effect options with a preferred repeat count.

iOS 17.0–18.4DeprecatediPadOS 17.0–18.4DeprecatedMac CatalystmacOS 14.0–15.4DeprecatedtvOS 17.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 10.0–11.4Deprecated

``` source
static func `repeat`(_ count: Int?) -> SymbolEffectOptions
```

## Parameters 

`count`  

The preferred number of times to play the effect, or `nil` to request the default number of times. The function may clamp very large or small values.

## Return Value

A new set of effect options with the preferred repeat count.

## See Also

### Configuring repeating effects

var repeating: SymbolEffectOptions

A set of effect options that prefers to repeat indefinitely.

static var repeating: SymbolEffectOptions

A default set of effect options that prefers to repeat indefinitely.

var nonRepeating: SymbolEffectOptions

A set of effect options that prefers to not repeat.

static var nonRepeating: SymbolEffectOptions

A default set of effect options that prefers to not repeat.

func `repeat`(Int?) -> SymbolEffectOptions

Creates a set of effect options with a preferred repeat count.

