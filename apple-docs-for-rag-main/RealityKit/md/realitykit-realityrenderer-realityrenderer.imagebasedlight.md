

- RealityKit
- RealityRenderer
-  RealityRenderer.ImageBasedLight 

Structure

# RealityRenderer.ImageBasedLight

Describe the lighting properties for the scene.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct ImageBasedLight
```

## Topics

### Instance Properties

var intensityExponent: Float

The intensity value of the light. The intensity modulates the intensity specified in the diffuse and specular textures An intensity of 0 means using the diffuse/specular intensities as-is Otherwise the intensity is multiplied by 2^intensity

var resource: EnvironmentResource?

The corresponding `EnvironmentResource` used for your Image Based Light.

## See Also

### Metal workflow rendering

class RealityRenderer

A renderer that displays a RealityKit scene in an existing Metal workflow.

struct CameraSettings

Settings for rendering with a camera.

struct CameraOutput

Output produced by rendering with a camera.

struct MetalEventAction

The structure describing an event and value to be signaled or waited for.

struct EntityCollection

A collection of entities in a RealityRenderer.

