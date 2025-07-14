

- RealityKit
- HoverEffectComponent
-  HoverEffectComponent.HoverEffect 

Structure

# HoverEffectComponent.HoverEffect

An effect that applies when a person looks at or directly touches the entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct HoverEffect
```

## Topics

### Type Methods

static func highlight(HoverEffectComponent.HighlightHoverEffectStyle) -> HoverEffectComponent.HoverEffect

Returns a hover effect style that uniformly highlights the entity and also applies a feathered spotlight effect.

static func shader(HoverEffectComponent.ShaderHoverEffectInputs) -> HoverEffectComponent.HoverEffect

Returns a hover effect style that applies hover state data to a custom shader that applies to the entity’s model.

static func spotlight(HoverEffectComponent.SpotlightHoverEffectStyle) -> HoverEffectComponent.HoverEffect

Returns a hover effect that displays a feathered spotlight on the entity where the current hover location is.

