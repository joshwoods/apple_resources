

- RealityKit
- ModelDebugOptionsComponent
- ModelDebugOptionsComponent.VisualizationMode
-  ModelDebugOptionsComponent.VisualizationMode.clearcoat 

Case

# ModelDebugOptionsComponent.VisualizationMode.clearcoat

A mode that displays the clearcoat channel of a material as the surface color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
case clearcoat
```

## Discussion

Add a ModelDebugOptionsComponent with a visualization mode of `clearcoat` to an entity to tell RealityKit to draw the entity’s clearcoat values as its surface color. A clearcoat is a way to render objects that appear to have a transparent coating or veneer, such as the surface of a car with a coat of wax or items shrinkwrapped in clear plastic. RealityKit draws clearcoat values as a grayscale value from black (`0.0`) to white (`1.0`), with black representing parts of the entity that don’t use clearcoat.

RealityKit calculates clearcoat for entities with a SimpleMaterial and for entities imported from a USDZ file. For other entities, this option has no effect.

Here’s how to enable roughness visualization for an entity:

```
if let television = try? await ModelEntity(named: "tv_retro") {
    let component = ModelDebugOptionsComponent(visualizationMode: .clearcoat)
    television.components.set(component)
}
```

| ModelDebugOptionsComponent.VisualizationMode.none | `clearcoat` |
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

case specular

A mode that displays en entity’s shininess as its surface color.

case emissive

A mode that displays the emissive channel of a material as the surface color.

case clearcoatRoughness

A mode that displays the clearcoat roughness channel of a material as the surface color.

case lightingDiffuse

A mode that displays the intensity of indirect light hitting the entity as its surface color.

