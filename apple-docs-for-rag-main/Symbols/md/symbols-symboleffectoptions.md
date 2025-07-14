

- Symbols
-  SymbolEffectOptions 

Structure

# SymbolEffectOptions

Options that configure how effects apply to symbol-based images.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct SymbolEffectOptions
```

## Topics

### Accessing effect options

static var `default`: SymbolEffectOptions

The default set of effect options.

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

static func `repeat`(Int?) -> SymbolEffectOptions

A default set of effect options with a preferred repeat count.

### Configuring effect speed

func speed(Double) -> SymbolEffectOptions

Creates a set of effect options with a preferred speed multiplier.

static func speed(Double) -> SymbolEffectOptions

A default set of effect options with a preferred speed multiplier.

### Structures

struct RepeatBehavior

### Instance Methods

func `repeat`(SymbolEffectOptions.RepeatBehavior) -> SymbolEffectOptions

### Type Methods

static func `repeat`(SymbolEffectOptions.RepeatBehavior) -> SymbolEffectOptions

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

