

- ARKit
- ARBodyTrackingConfiguration
-  wantsHDREnvironmentTextures 

Instance Property

# wantsHDREnvironmentTextures

A flag that instructs ARKit to create environment textures in HDR format.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var wantsHDREnvironmentTextures: Bool { get set }
```

## Discussion

The default value is true. If your renderer supports HDR environment textures, this feature effects more realistic reflections.

RealityKit and SceneKit both support HDR environment textures. For more information, see Adding realistic reflections to an AR experience.

## See Also

### Adding Realistic Reflections

var environmentTexturing: ARWorldTrackingConfiguration.EnvironmentTexturing

The behavior ARKit uses for generating environment textures.

