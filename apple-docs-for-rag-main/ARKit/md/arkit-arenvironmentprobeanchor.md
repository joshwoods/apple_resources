

- ARKit
-  AREnvironmentProbeAnchor 

Class

# AREnvironmentProbeAnchor

An object that provides environmental lighting information for a specific area of space in a world-tracking AR session.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class AREnvironmentProbeAnchor
```

## Overview

Environment textures depict the view in all directions from a specific point in a scene. In 3D asset rendering, environment textures are the basis for image-based lighting algorithms where surfaces can realistically reflect light from their surroundings. ARKit can generate environment textures during an AR session using camera imagery, allowing SceneKit or a custom-rendering engine to provide realistic image-based lighting for virtual objects in your AR experience.

To enable texture map generation for an AR session, set the environmentTexturing property:

- With ARWorldTrackingConfiguration.EnvironmentTexturing.manual environment texturing, you identify points in the scene for which you want light probe texture maps by creating AREnvironmentProbeAnchor objects and adding them to the session.

- With ARWorldTrackingConfiguration.EnvironmentTexturing.automatic environment texturing, ARKit automatically creates, positions, and adds AREnvironmentProbeAnchor objects to the session.

In both cases, ARKit automatically generates environment textures as the session collects camera imagery. Use a delegate method such as session(_:didUpdate:) to find out when a texture is available, and access it from the anchor’s environmentTexture property.

If you display AR content using ARSCNView and the automaticallyUpdatesLighting option, SceneKit automatically retrieves AREnvironmentProbeAnchor texture maps and uses them to light the scene.

## Topics

### Creating Probe Anchors

init(transform: simd_float4x4, extent: simd_float3)

Creates a new environment probe anchor.

init(name: String, transform: simd_float4x4, extent: simd_float3)

Creates a new anchor object with a descriptive name.

### Accessing Texture Maps

var environmentTexture: (any MTLTexture)?

A cube-map texture that represents the view in all directions from the probe anchor’s position.

### Examining a Probe Anchor

var extent: simd_float3

The area around the anchor’s position that contains the texture.

## Relationships

### Inherits From

- ARAnchor

### Conforms To

- ARAnchorCopying
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Lighting Effects

Adding realistic reflections to an AR experience

Use ARKit to generate environment probe textures from camera imagery and render reflective virtual objects.

class ARLightEstimate

Estimated scene lighting information associated with a captured video frame in an AR session.

class ARDirectionalLightEstimate

Estimated environmental lighting information associated with a captured video frame in a face-tracking AR session.

