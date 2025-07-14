

- RealityKit
- ModelDebugOptionsComponent
- ModelDebugOptionsComponent.VisualizationMode
-  ModelDebugOptionsComponent.VisualizationMode.bitangent 

Case

# ModelDebugOptionsComponent.VisualizationMode.bitangent

A mode that displays the surface bitangent vectors as a color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
case bitangent
```

## Discussion

Add a ModelDebugOptionsComponent with a visualization mode of `bitangent` to an entity to tell RealityKit to draw that entity’s calculated surface bitangent vectors as its surface color. A bitangent vector is an imaginary line that’s orthagonal to both the `normal` and `tangent` vectors. RealityKit draws a bitangent vector by using its `X`, `Y`, and `Z` values as the `R`, `G`, and `B` components of the color.

RealityKit calculates bitangents for entities with a VideoMaterial, UnlitMaterial, or SimpleMaterial as well as for entities imported from a USDZ file. If an entity doesn’t fall within those parameters, this option has no effect on the rendering.

Here’s how to enable bitangent visualization for an entity:

```
if let television = try? await ModelEntity(named: "tv_retro") {
    let component = ModelDebugOptionsComponent(visualizationMode: .bitangent)
    television.components.set(component)
}
```

| ModelDebugOptionsComponent.VisualizationMode.none | `bitangent` |
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

