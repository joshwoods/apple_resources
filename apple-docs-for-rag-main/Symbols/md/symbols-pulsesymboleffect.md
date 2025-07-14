

- Symbols
-  PulseSymbolEffect 

Structure

# PulseSymbolEffect

A type that fades the opacity of some or all layers in a symbol-based image.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct PulseSymbolEffect
```

## Overview

A pulse animation applies an opacity ramp to the layers in a symbol. You can choose to animate only layers marked as “always-pulses” or all layers simultaneously. Participating layers reduce their opacity to a minimum value before returning to fully opaque.

Important

Because SwiftUI is a state-driven framework, you pass a `value` parameter when adding discrete effects, like bounce. You trigger the animation by changing the `value` parameter. Because AppKit and UIKit are event-driven frameworks, discrete effects animate automatically when added to an image view.

```
// Add an effect in SwiftUI.
@State private var value1 = 0
@State private var value2 = 0
var body: some View {
    HStack {
        Image(systemName: "person.text.rectangle")
            // Pulse only layers marked as "always-pulse."
            .symbolEffect(.pulse, value: value1)
            .onTapGesture {
                value1 += 1
            }
        Image(systemName: "person.text.rectangle")
            // Pulse all layers three times simultaneously.
            .symbolEffect(.pulse.wholeSymbol, options: .repeat(3), value: value2)
            .onTapGesture {
                value2 += 1
            }
    }
}
```

```
// Add an effect in AppKit and UIKit.
// Pulse only layers marked as "always-pulse."
imageView1.addSymbolEffect(.pulse.byLayer, options: .nonRepeating)

// Pulse all layers three times simultaneously.
imageView2.addSymbolEffect(.pulse.wholeSymbol, options: .repeat(3))
```

## Topics

### Determining effect scope

var byLayer: PulseSymbolEffect

An effect requesting an animation that pulses only the layers marked to always pulse.

var wholeSymbol: PulseSymbolEffect

An effect requesting an animation that pulses all layers simultaneously.

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

struct BounceSymbolEffect

A type that applies a transitory scaling effect, or bounce, to the layers in a symbol-based image separately or as a whole.

struct DisappearSymbolEffect

A type that makes the layers of a symbol-based image disappear separately or as a whole.

struct ReplaceSymbolEffect

A type that replaces the layers of one symbol-based image with those of another.

struct ScaleSymbolEffect

A type that scales the layers in a symbol-based image separately or as a whole.

struct VariableColorSymbolEffect

A type that replaces the opacity of variable layers in a symbol-based image in a repeatable sequence.

struct BreatheSymbolEffect

struct RotateSymbolEffect

struct WiggleSymbolEffect

