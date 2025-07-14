

- RealityKit
- ModelDebugOptionsComponent
- ModelDebugOptionsComponent.VisualizationMode
-  ModelDebugOptionsComponent.VisualizationMode.finalColor 

Case

# ModelDebugOptionsComponent.VisualizationMode.finalColor

A mode that displays the entity’s calculated color, ignoring transparency.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
case finalColor
```

## Discussion

Add a ModelDebugOptionsComponent with a visualization mode of `finalColor` to an entity to tell RealityKit to draw that entity’s calculated surface color with no transparency. This option causes RealityKit to render the object as if it were fully opaque. For entities that don’t use transparency, this option has no affect.

Here’s how to enable final color visualization for an entity:

```
if let television = try? await ModelEntity(named: "tv_retro") {
    let component = ModelDebugOptionsComponent(visualizationMode: .finalColor)
    television.components.set(component)
}
```

| ModelDebugOptionsComponent.VisualizationMode.none | `finalColor` |
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

