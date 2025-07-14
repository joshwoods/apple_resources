

- RealityKit
- HoverEffectComponent
-  HoverEffectComponent.ShaderHoverEffectInputs 

Structure

# HoverEffectComponent.ShaderHoverEffectInputs

A type that configures the visual aspects of a hover effect that applies a custom material

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ShaderHoverEffectInputs
```

## Topics

### Operators

static func == (HoverEffectComponent.ShaderHoverEffectInputs, HoverEffectComponent.ShaderHoverEffectInputs) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(fadeInDuration: TimeInterval, fadeOutDuration: TimeInterval)

### Instance Properties

var fadeInDuration: TimeInterval

The time it takes in seconds for the effect to fade in.

var fadeOutDuration: TimeInterval

The time it takes in seconds for the effect to fade out.

### Type Properties

static let `default`: HoverEffectComponent.ShaderHoverEffectInputs

The default style initializes the fade-in and fade-out durations to match the durations of the default spotlight.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

