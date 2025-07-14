

- Symbols
-  ScaleSymbolEffect 

Structure

# ScaleSymbolEffect

A type that scales the layers in a symbol-based image separately or as a whole.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ScaleSymbolEffect
```

## Overview

A scale animation draws attention to a symbol by changing the symbol’s scale indefinitely. You can choose to scale the symbol up or down.

## Topics

### Accessing symbol effects

var down: ScaleSymbolEffect

An effect that scales the symbol down.

var up: ScaleSymbolEffect

An effect that scales the symbol up.

### Determining effect scope

var byLayer: ScaleSymbolEffect

An effect that scales each layer separately.

var wholeSymbol: ScaleSymbolEffect

An effect that scales all layers simultaneously.

### Accessing the configuration

var configuration: SymbolEffectConfiguration

The configuration for the effect.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- IndefiniteSymbolEffect
- Sendable
- SymbolEffect

## See Also

### Symbol effect types

struct AppearSymbolEffect

A type that makes the layers of a symbol-based image appear separately or as a whole.

struct AutomaticSymbolEffect

A type that applies the default animation to a symbol-based image in a context-sensitive manner.

struct BounceSymbolEffect

A type that applies a transitory scaling effect, or bounce, to the layers in a symbol-based image separately or as a whole.

struct DisappearSymbolEffect

A type that makes the layers of a symbol-based image disappear separately or as a whole.

struct PulseSymbolEffect

A type that fades the opacity of some or all layers in a symbol-based image.

struct ReplaceSymbolEffect

A type that replaces the layers of one symbol-based image with those of another.

struct VariableColorSymbolEffect

A type that replaces the opacity of variable layers in a symbol-based image in a repeatable sequence.

struct BreatheSymbolEffect

struct RotateSymbolEffect

struct WiggleSymbolEffect

