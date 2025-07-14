

- RealityKit
- ModelDebugOptionsComponent
- ModelDebugOptionsComponent.VisualizationMode
-  ModelDebugOptionsComponent.VisualizationMode.specular 

Case

# ModelDebugOptionsComponent.VisualizationMode.specular

A mode that displays en entity’s shininess as its surface color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
case specular
```

## Discussion

Add a ModelDebugOptionsComponent with a visualization mode of `specular` to an entity to tell RealityKit to draw the entity’s calculated specularity as its surface color. RealityKit uses `specular` to calculate bright highlights caused by shiny surfaces reflecting light. RealityKit draws the specularity value as a grayscale value from black (`0.0`) to white (`1.0`).

Note

In most cases, RealityKit calculates specular highlights based on an entity’s `roughness` and `metallic` values, and not its `specular` value, which is usually `0.0`. As a result, this mode causes most entities to render in solid black. Only entities that need highlights in addition to the ones RealityKit calculates from `roughness` and `metallic` need `specular` values greater than zero. Examples of entities that might use `specular` to create supplemental highlights are gemstones and cut glass.

RealityKit calculates specularity for entities with a SimpleMaterial and for entities imported from a USDZ file. For other entities, this option has no effect.

Here’s how to enable ambient occlusion visualization for an entity:

```
if let television = try? await ModelEntity(named: "tv_retro") {
    let component = ModelDebugOptionsComponent(visualizationMode: .specular)
    television.components.set(component)
}
```

| ModelDebugOptionsComponent.VisualizationMode.none | `specular` |
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

case ambientOcclusion

A mode that displays the calculated ambient occlusion value as the surface color.

case emissive

A mode that displays the emissive channel of a material as the surface color.

case clearcoat

A mode that displays the clearcoat channel of a material as the surface color.

case clearcoatRoughness

A mode that displays the clearcoat roughness channel of a material as the surface color.

case lightingDiffuse

A mode that displays the intensity of indirect light hitting the entity as its surface color.

