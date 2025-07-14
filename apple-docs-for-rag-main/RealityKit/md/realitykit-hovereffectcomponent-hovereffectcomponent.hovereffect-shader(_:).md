

- RealityKit
- HoverEffectComponent
- HoverEffectComponent.HoverEffect
-  shader(\_:) 

Type Method

# shader(\_:)

Returns a hover effect style that applies hover state data to a custom shader that applies to the entity’s model.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func shader(_ inputs: HoverEffectComponent.ShaderHoverEffectInputs) -> HoverEffectComponent.HoverEffect
```

## Parameters 

`inputs`  

A HoverEffectComponent.ShaderHoverEffectInputs instance that allows you to customize various aspects of this hover effect.

## Discussion

The custom shader can be either MaterialX or CustomMaterial.

Warning

This style doesn’t display anything without an appropriate custom shader.

