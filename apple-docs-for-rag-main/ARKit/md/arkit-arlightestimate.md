

- ARKit
-  ARLightEstimate 

Class

# ARLightEstimate

Estimated scene lighting information associated with a captured video frame in an AR session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARLightEstimate
```

## Overview

If you enable the isLightEstimationEnabled setting, ARKit provides light estimates in the lightEstimate property of each ARFrame it delivers.

If you render your own overlay graphics for the AR scene, you can use this information in shading algorithms to help make those graphics match the real-world lighting conditions of the scene captured by the camera. The ARSCNView class automatically uses this information to configure SceneKit lighting.

## Topics

### Examining Light Parameters

var ambientIntensity: CGFloat

The estimated intensity, in lumens, of ambient light throughout the scene.

var ambientColorTemperature: CGFloat

The estimated color temperature, in degrees Kelvin, of ambient light throughout the scene.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ARDirectionalLightEstimate

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

class ARDirectionalLightEstimate

Estimated environmental lighting information associated with a captured video frame in a face-tracking AR session.

