

- ARKit
-  AROrientationTrackingConfiguration 

Class

# AROrientationTrackingConfiguration

A configuration that tracks only the device’s orientation using the rear-facing camera.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class AROrientationTrackingConfiguration
```

## Overview

All AR configurations establish a correspondence between the real world the device inhabits and a virtual 3D coordinate space where you can model content. When your app displays that content together with a live camera image, the user experiences the illusion that your virtual content is part of the real world.

Creating and maintaining this correspondence between spaces requires tracking the device’s motion. The AROrientationTrackingConfiguration class tracks the device’s movement with three degrees of freedom (3DOF): specifically, the three rotation axes (roll, pitch, and yaw).

This basic level of motion tracking can create limited AR experiences: A virtual object can appear to be part of the real world, even as the user rotates the device to look above, below, or beside that object. However, this configuration cannot track movement of the device: non-trivially changing the device’s position breaks the AR illusion, causing virtual content to appear to drift relative to the real world. For example, the user cannot walk around to see the sides and back of a virtual object. Additionally, 3DOF tracking does not support plane detection or hit testing.

Important

Because 3DOF tracking creates limited AR experiences, you should generally not use the AROrientationTrackingConfiguration class directly. Instead, use ARWorldTrackingConfiguration for six degrees of freedom (6DOF) plane detection and hit testing. Use 3DOF tracking only as a fallback in situations where 6DOF tracking is temporarily unavailable.

## Topics

### Creating a Configuration

init()

Initializes a new orientation tracking configuration.

### Managing Device Camera Behavior

var isAutoFocusEnabled: Bool

A Boolean value that determines whether the device camera uses fixed focus or autofocus behavior.

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

class ARPositionalTrackingConfiguration

A configuration that tracks only the device’s position in 3D space.

