

- RealityKit
- ModelDebugOptionsComponent
- ModelDebugOptionsComponent.VisualizationMode
-  ModelDebugOptionsComponent.VisualizationMode.clearcoatNormal 

Case

# ModelDebugOptionsComponent.VisualizationMode.clearcoatNormal

A mode that displays the clearcoat normal of a material as the surface color.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case clearcoatNormal
```

## Discussion

Adding a ModelDebugOptionsComponent with a visualization mode of `clearcoatNormal` to an entity tells RealityKit to draw the world space clearcoat normal as its surface color. RealityKit draws the xyz value as a rgb color value after it has been transformed from tangent to world space.

Here’s how to enable clearcoat normal visualization for an entity:

```
if let television = try? await ModelEntity(named: "tv_retro") {
    let component = ModelDebugOptionsComponent(visualizationMode: .clearcoatNormal)
    television.components.set(component)
}
```

| ModelDebugOptionsComponent.VisualizationMode.none | `clearcoatNormal` |
|----|----|
|  |  |

