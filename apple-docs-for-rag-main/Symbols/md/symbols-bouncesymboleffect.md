

- Symbols
-  BounceSymbolEffect 

Structure

# BounceSymbolEffect

A type that applies a transitory scaling effect, or bounce, to the layers in a symbol-based image separately or as a whole.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct BounceSymbolEffect
```

## Overview

A bounce animation draws attention to a symbol by applying a brief scaling operation to the symbol’s layers. You can choose to scale the symbol up or down as it bounces.

Important

Because SwiftUI is a state-driven framework, you pass a `value` parameter when adding discrete effects, like bounce. You trigger the animation by changing the `value` parameter. Because AppKit and UIKit are event-driven frameworks, discrete effects animate automatically when added to an image view.

```
// Add an effect in SwiftUI.
@State private var value1 = 0
@State private var value2 = 0
var body: some View {
    HStack {
        Image(systemName: "arrow.up.circle")
            // Bounce with a scale-up animation.
            .symbolEffect(.bounce.up, value: value1)
            .onTapGesture {
                value1 += 1
            }
        Image(systemName: "arrow.down.circle")
            // Bounce three times with a scale-down animation.
            .symbolEffect(.bounce.down, options: .repeat(3), value: value2)
            .onTapGesture {
                value2 += 1
            }
    }
}
```

```
// Add an effect in AppKit and UIKit.
// Bounce with a scale-up animation.
imageView1.addSymbolEffect(.bounce.up)

// Bounce three times with a scale-down animation.
imageView2.addSymbolEffect(.bounce.down, options: .repeat(3))
```

## Topics

### Accessing symbol effects

var down: BounceSymbolEffect

An effect that bounces the symbol downward.

var up: BounceSymbolEffect

An effect that bounces the symbol upward.

### Determining effect scope

var byLayer: BounceSymbolEffect

An effect that bounces each layer separately.

var wholeSymbol: BounceSymbolEffect

An effect that bounces all layers simultaneously.

### Accessing the configuration

var configuration: SymbolEffectConfiguration

The configuration for the effect.

## Relationships

### Conforms To

- Copyable
- DiscreteSymbolEffect
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

