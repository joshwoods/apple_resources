

- RealityKit
- ModelDebugOptionsComponent
- ModelDebugOptionsComponent.VisualizationMode
-  ModelDebugOptionsComponent.VisualizationMode.finalAlpha 

Case

# ModelDebugOptionsComponent.VisualizationMode.finalAlpha

A mode that displays the entity’s calculated transparency as its surface color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
case finalAlpha
```

## Discussion

Add a ModelDebugOptionsComponent with a visualization mode of `finalAlpha` to an entity to tell RealityKit to draw that entity’s alpha value as its surface color. RealityKit draws the alpha value as a grayscale value from black (`0.0`) to white (`1.0`), meaning the more transparent a part of the entity is, the darker RealityKit draws it.

RealityKit calculates final alpha values for entities with a VideoMaterial, UnlitMaterial, SimpleMaterial as well as for entities imported from a USDZ file. If an entity doesn’t fall within those parameters, this option has no effect on the rendering.

Here’s how to enable alpha visualization for an entity:

```
if let television = try? await ModelEntity(named: "tv_retro") {
    let component = ModelDebugOptionsComponent(visualizationMode: .finalAlpha)
    television.components.set(component)
}
```

| ModelDebugOptionsComponent.VisualizationMode.none | `finalAlpha` |
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

