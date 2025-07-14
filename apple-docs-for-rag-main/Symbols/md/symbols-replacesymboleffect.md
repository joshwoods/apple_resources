

- Symbols
-  ReplaceSymbolEffect 

Structure

# ReplaceSymbolEffect

A type that replaces the layers of one symbol-based image with those of another.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ReplaceSymbolEffect
```

## Overview

A replace transition animates the change from one symbol image to another. You choose from one of the predefined scaling animations: Down-Up, Off-Up, and Up-Up.

Down-Up  
The initial symbol scales down as it’s removed, and the new symbol scales up as it’s added.

Off-Up  
The initial symbol is removed with no animation, and the new symbol scales up as it’s added.

Up-Up  
The initial symbol scales up as it’s removed, and the new symbol scales up as it’s added.

## Topics

### Accessing symbol effects

var downUp: ReplaceSymbolEffect

An effect that replaces a symbol by scaling it down, and scaling a different symbol up.

var offUp: ReplaceSymbolEffect

An effect that replaces a symbol by removing it, and scaling a different symbol up.

var upUp: ReplaceSymbolEffect

An effect that replaces a symbol by scaling it up, and scaling a different symbol up.

### Determining effect scope

var byLayer: ReplaceSymbolEffect

An effect that replaces each layer separately.

var wholeSymbol: ReplaceSymbolEffect

An effect that replaces all layers simultaneously.

### Accessing the configuration

var configuration: SymbolEffectConfiguration

The configuration for the effect.

### Structures

struct MagicReplace

### Instance Methods

func magic(fallback: ReplaceSymbolEffect) -> ReplaceSymbolEffect.MagicReplace

### Type Properties

static var downUp: ReplaceSymbolEffect

static var offUp: ReplaceSymbolEffect

static var upUp: ReplaceSymbolEffect

## Relationships

### Conforms To

- ContentTransitionSymbolEffect
- Copyable
- Equatable
- Hashable
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

struct ScaleSymbolEffect

A type that scales the layers in a symbol-based image separately or as a whole.

struct VariableColorSymbolEffect

A type that replaces the opacity of variable layers in a symbol-based image in a repeatable sequence.

struct BreatheSymbolEffect

struct RotateSymbolEffect

struct WiggleSymbolEffect

