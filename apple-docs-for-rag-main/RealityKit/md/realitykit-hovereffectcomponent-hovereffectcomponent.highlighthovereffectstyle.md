

- RealityKit
- HoverEffectComponent
-  HoverEffectComponent.HighlightHoverEffectStyle 

Structure

# HoverEffectComponent.HighlightHoverEffectStyle

A type that configures the visual aspects of a highlight hover effect for an entity

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct HighlightHoverEffectStyle
```

## Topics

### Operators

static func == (HoverEffectComponent.HighlightHoverEffectStyle, HoverEffectComponent.HighlightHoverEffectStyle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(color: NSColor?, strength: Float)

Creates a new highlight effect with a color and strength.

init(color: UIColor?, strength: Float)

Creates a new highlight effect with a color and strength.

init(color: NSColor?, strength: Float, opacityFunction: HoverEffectComponent.OpacityFunction)

Creates a new highlight effect with a color and strength.

init(color: UIColor?, strength: Float, opacityFunction: HoverEffectComponent.OpacityFunction)

Creates a new highlight effect with a color and strength.

### Instance Properties

var color: NSColor

The color tint for the highlight hover effect.

var color: UIColor

The color tint for the highlight hover effect.

var opacityFunction: HoverEffectComponent.OpacityFunction

The blending technique the hover effect applies to the entity’s base material.

var strength: Float

A floating-point value that represents the intensity of the effect.

### Type Properties

static let `default`: HoverEffectComponent.HighlightHoverEffectStyle

The default style applies a white uniform glow to the affect entity as well as a white spotlight glow at the hover location

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

