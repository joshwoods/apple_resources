

- ARKit
-  ARDirectionalLightEstimate 

Class

# ARDirectionalLightEstimate

Estimated environmental lighting information associated with a captured video frame in a face-tracking AR session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARDirectionalLightEstimate
```

## Overview

When you run a face tracking AR session (see ARFaceTrackingConfiguration) with the isLightEstimationEnabled property set to true, ARKit uses the detected face as a light probe to estimate the directional lighting environment in the scene. The lightEstimate property of each frame vended by the session contains an ARDirectionalLightEstimate instance containing this information.

If you render your own overlay graphics for the AR scene, you can use this information in shading algorithms to help make those graphics match the real-world lighting conditions of the scene captured by the camera. (The ARSCNView class automatically uses this information to configure SceneKit lighting.)

## Topics

### Examining Light Parameters

var sphericalHarmonicsCoefficients: Data

Data describing the estimated lighting environment in all directions.

var primaryLightDirection: simd_float3

A vector indicating the orientation of the strongest directional light source in the scene.

var primaryLightIntensity: CGFloat

The estimated intensity, in lumens, of the strongest directional light source in the scene.

## Relationships

### Inherits From

- ARLightEstimate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Lighting Effects

Adding realistic reflections to an AR experience

Use ARKit to generate environment probe textures from camera imagery and render reflective virtual objects.

class AREnvironmentProbeAnchor

An object that provides environmental lighting information for a specific area of space in a world-tracking AR session.

class ARLightEstimate

Estimated scene lighting information associated with a captured video frame in an AR session.

