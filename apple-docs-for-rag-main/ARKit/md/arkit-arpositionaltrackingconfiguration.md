

- ARKit
-  ARPositionalTrackingConfiguration 

Class

# ARPositionalTrackingConfiguration

A configuration that tracks only the device’s position in 3D space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARPositionalTrackingConfiguration
```

## Overview

Enables 6 degrees of freedom tracking of the iOS device by running the camera at lowest possible resolution and frame rate. Use this configuration when you don’t need to parse the camera feed, such as for example, virtual reality scenarios.

## Topics

### Creating a Configuration

init()

Creates a new positional tracking configuration.

var initialWorldMap: ARWorldMap?

The state from a previous AR session to attempt to resume with this session configuration.

### Detecting Real-World Surfaces

var planeDetection: ARWorldTrackingConfiguration.PlaneDetection

A value that specifies if and how the session automatically attempts to detect flat surfaces in the camera-captured image.

## Relationships

### Inherits From

- ARConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Spatial Tracking

Understanding World Tracking

Discover features and best practices for building rear-camera AR experiences.

class ARWorldTrackingConfiguration

A configuration that tracks the position of a device in relation to objects in the environment.

class ARGeoTrackingConfiguration

A configuration that tracks locations with GPS, map data, and a device’s compass.

class AROrientationTrackingConfiguration

A configuration that tracks only the device’s orientation using the rear-facing camera.

