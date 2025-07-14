

- Symbols
-  AppearSymbolEffect 

Structure

# AppearSymbolEffect

A type that makes the layers of a symbol-based image appear separately or as a whole.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct AppearSymbolEffect
```

## Overview

An appear transition causes a symbol to become visible using a scaling animation. You can choose to scale the image up or down and to animate the symbol by individual layers or as a whole.

## Topics

### Accessing symbol effects

var down: AppearSymbolEffect

An effect that makes the symbol scale down as it appears.

var up: AppearSymbolEffect

An effect that makes the symbol scale up as it appears.

### Determining effect scope

var byLayer: AppearSymbolEffect

An effect that makes each layer appear separately.

var wholeSymbol: AppearSymbolEffect

An effect that makes all layers appear simultaneously.

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
- TransitionSymbolEffect

## See Also

### Symbol effect types

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

struct ScaleSymbolEffect

A type that scales the layers in a symbol-based image separately or as a whole.

struct VariableColorSymbolEffect

A type that replaces the opacity of variable layers in a symbol-based image in a repeatable sequence.

struct BreatheSymbolEffect

struct RotateSymbolEffect

struct WiggleSymbolEffect

