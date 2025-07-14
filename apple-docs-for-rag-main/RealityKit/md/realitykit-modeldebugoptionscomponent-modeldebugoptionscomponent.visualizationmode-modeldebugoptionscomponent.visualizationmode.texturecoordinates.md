

- RealityKit
- ModelDebugOptionsComponent
- ModelDebugOptionsComponent.VisualizationMode
-  ModelDebugOptionsComponent.VisualizationMode.textureCoordinates 

Case

# ModelDebugOptionsComponent.VisualizationMode.textureCoordinates

A mode that displays the texture coordinates as a color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
case textureCoordinates
```

## Discussion

Adding a ModelDebugOptionsComponent with a visualization mode of `textureCoordinates` to an entity tells RealityKit to draw that entity’s UV texture coordinates as its surface color. RealityKit draws the texture coordinates by using its `U` and `V` values as the `R` and `G` components of the color, using a value of `0` for the color’s `B` component.

RealityKit calculates texture coordinates for entities with a VideoMaterial, UnlitMaterial, SimpleMaterial as well as for entities imported from a USDZ file. If an entity doesn’t fall within those parameters, this option has no effect on the rendering.

Here’s how to enable UV texture coordinate visualization for an entity:

```
if let television = try? await ModelEntity(named: "tv_retro") {
    let component = ModelDebugOptionsComponent(visualizationMode: .textureCoordinates)
    television.components.set(component)
}
```

| ModelDebugOptionsComponent.VisualizationMode.none | `textureCoordinates` |
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

