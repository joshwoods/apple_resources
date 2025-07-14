

- ARKit
- ARWorldTrackingConfiguration
-  ARWorldTrackingConfiguration.EnvironmentTexturing 

Enumeration

# ARWorldTrackingConfiguration.EnvironmentTexturing

The available environment texturing options for world tracking.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
enum EnvironmentTexturing
```

## Discussion

Environment textures are cube-map textures that depict the view in all directions from a specific point in a scene. In 3D asset rendering, environment textures are the basis for image-based lighting algorithms where surfaces can realistically reflect light from their surroundings. ARKit generates environment textures during an AR session using camera imagery, allowing SceneKit or a custom-rendering engine to provide realistic image-based lighting for virtual objects in your AR experience.

To enable texture map generation for your configuration, change this property (from its default value of ARWorldTrackingConfiguration.EnvironmentTexturing.none):

- With ARWorldTrackingConfiguration.EnvironmentTexturing.manual environment texturing, you identify points in the scene for which you want light probe texture maps by creating AREnvironmentProbeAnchor objects and adding them to the session.

- With ARWorldTrackingConfiguration.EnvironmentTexturing.automatic environment texturing, ARKit automatically creates, positions, and adds AREnvironmentProbeAnchor objects to the session.

In both cases, ARKit automatically generates environment textures as the session collects camera imagery. Use a delegate method such as session(_:didUpdate:) to find out when a texture is available, and access it from the anchor’s environmentTexture property.

If you display AR content using ARSCNView and the automaticallyUpdatesLighting option, SceneKit automatically retrieves AREnvironmentProbeAnchor texture maps and uses them to light the scene.

## Topics

### Enumeration Cases

case automatic

The framework automatically determines when and where to generate environment textures.

case manual

The framework generates environment textures only for probe anchors you explicitly add to the session.

case none

The framework doesn’t generate environment textures.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Realistic Reflections

var environmentTexturing: ARWorldTrackingConfiguration.EnvironmentTexturing

An option that determines how the framework generates environment textures.

class AREnvironmentProbeAnchor

An object that provides environmental lighting information for a specific area of space in a world-tracking AR session.

var wantsHDREnvironmentTextures: Bool

A flag that instructs the framework to create environment textures in HDR format.

