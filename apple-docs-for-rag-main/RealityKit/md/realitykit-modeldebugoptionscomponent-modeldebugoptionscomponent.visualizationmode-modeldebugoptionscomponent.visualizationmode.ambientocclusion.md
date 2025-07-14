

- RealityKit
- ModelDebugOptionsComponent
- ModelDebugOptionsComponent.VisualizationMode
-  ModelDebugOptionsComponent.VisualizationMode.ambientOcclusion 

Case

# ModelDebugOptionsComponent.VisualizationMode.ambientOcclusion

A mode that displays the calculated ambient occlusion value as the surface color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
case ambientOcclusion
```

## Discussion

Add a ModelDebugOptionsComponent with a visualization mode of `ambientOcclusion` to an entity to tell RealityKit to draw the calculated ambient occlusion values as the entity’s surface color. Ambient occlusion represents the entity’s exposure to ambient light. RealityKit draws ambient occlusion values as a grayscale value from black (`0.0`) to white (`1.0`), rendering flat surface areas in white, and crevices, dents, and recessed areas in darker shades.

RealityKit calculates ambient occlusion for entities with a SimpleMaterial and for entities imported from a USDZ file. For other entities, this option has no effect.

Here’s how to enable ambient occlusion visualization for an entity:

```
if let television = try? await ModelEntity(named: "tv_retro") {
    let component = ModelDebugOptionsComponent(visualizationMode: .ambientOcclusion)
    television.components.set(component)
}
```

| ModelDebugOptionsComponent.VisualizationMode.none | `ambientOcclusion` |
|----|----|
|  |  |

## See Also

### Visualization modes

case none

A mode that doesn’t display a visualization.

case normal

A mode that displays the normal vectors as a color.

case tangent

A mode that displays the surface tangent vectors as a color.

case bitangent

A mode that displays the surface bitangent vectors as a color.

case baseColor

A mode that displays the entity’s base color with no lighting or material properties applied.

case textureCoordinates

A mode that displays the texture coordinates as a color.

case finalColor

A mode that displays the entity’s calculated color, ignoring transparency.

case finalAlpha

A mode that displays the entity’s calculated transparency as its surface color.

case roughness

A mode that displays the shininess of a material as the surface color.

case metallic

A mode that displays the reflectiveness of an entity as its surface color.

case specular

A mode that displays en entity’s shininess as its surface color.

case emissive

A mode that displays the emissive channel of a material as the surface color.

case clearcoat

A mode that displays the clearcoat channel of a material as the surface color.

case clearcoatRoughness

A mode that displays the clearcoat roughness channel of a material as the surface color.

case lightingDiffuse

A mode that displays the intensity of indirect light hitting the entity as its surface color.

