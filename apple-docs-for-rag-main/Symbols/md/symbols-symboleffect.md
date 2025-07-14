

- Symbols
-  SymbolEffect 

Protocol

# SymbolEffect

A presentation effect that you apply to a symbol-based image.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol SymbolEffect : Hashable, Sendable
```

## Topics

### Effects

static var appear: AppearSymbolEffect

An animation that makes the layers of a symbol-based image appear separately or as a whole.

static var bounce: BounceSymbolEffect

An animation that applies a transitory scaling effect, or bounce, to the layers in a symbol-based image separately or as a whole.

static var disappear: DisappearSymbolEffect

An animation that makes the layers of a symbol-based image disappear separately or as a whole.

static var pulse: PulseSymbolEffect

An animation that fades the opacity of some or all layers in a symbol-based image.

static var scale: ScaleSymbolEffect

An animation that scales the layers in a symbol-based image separately or as a whole.

static var variableColor: VariableColorSymbolEffect

An animation that replaces the opacity of variable layers in a symbol-based image in a repeatable sequence.

static var breathe: BreatheSymbolEffect

static var rotate: RotateSymbolEffect

static var wiggle: WiggleSymbolEffect

### Accessing the configuration

var configuration: SymbolEffectConfiguration

A configuration for a symbol effect.

**Required**

struct SymbolEffectConfiguration

A type that specifies the configuration of a symbol effect.

### Type Properties

static var automatic: AutomaticSymbolEffect

A transition that applies the default animation to a symbol-based image in a context-sensitive manner.

static var replace: ReplaceSymbolEffect

An animation that replaces the layers of one symbol-based image with those of another.

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable

### Conforming Types

- AppearSymbolEffect
- AutomaticSymbolEffect
- BounceSymbolEffect
- BreatheSymbolEffect
- DisappearSymbolEffect
- PulseSymbolEffect
- ReplaceSymbolEffect
- ReplaceSymbolEffect.MagicReplace
- RotateSymbolEffect
- ScaleSymbolEffect
- VariableColorSymbolEffect
- WiggleSymbolEffect

## See Also

### Symbol effect protocols

protocol DiscreteSymbolEffect

An effect that performs a transient animation.

protocol IndefiniteSymbolEffect

An animation that continually affects a symbol until it’s disabled or removed.

protocol ContentTransitionSymbolEffect

An effect that animates between symbols or different configurations of the same symbol.

protocol TransitionSymbolEffect

An effect that animates a symbol in or out.

