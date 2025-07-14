

- ARKit
-  ARFaceTrackingConfiguration 

Class

# ARFaceTrackingConfiguration

A configuration that tracks facial movement and expressions using the front camera.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARFaceTrackingConfiguration
```

## Mentioned in 

Verifying Device Support and User Permission

Choosing Which Camera Feed to Augment

## Overview

A face-tracking configuration detects faces within 3 meters of the device’s front camera. When ARKit detects a face, it creates an ARFaceAnchor object that provides information about a person’s facial position, orientation, topology, and expressions.

Face tracking supports devices with Apple Neural Engine in iOS 14 and iPadOS 14 and requires a device with a TrueDepth camera on iOS 13 and iPadOS 13 and earlier. To determine whether the device supports face tracking, call isSupported on ARFaceTrackingConfiguration before attempting to use this configuration.

When you enable the isLightEstimationEnabled setting, a face-tracking configuration estimates directional and environmental lighting (an ARDirectionalLightEstimate object) by referring to the detected face as a light probe.

Note

Because face tracking provides your app with personal facial information, your app must include a privacy policy describing to users how you intend to use face tracking and face data. For details, see the Apple Developer Program License Agreement.

## Topics

### Creating a Configuration

init()

Creates a new face-tracking configuration.

### Enabling World Tracking

class var supportsWorldTracking: Bool

A Boolean value that indicates whether the iOS device supports tracking the user’s facial features in a world-tracking session.

var isWorldTrackingEnabled: Bool

A Boolean value that instructs a session to provide the app with the device’s six degrees of freedom pose during a face-tracking session.

### Tracking Multiple Faces

var maximumNumberOfTrackedFaces: Int

The number of faces to track during the session.

class var supportedNumberOfTrackedFaces: Int

The maximum number of faces that the framework can track.

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

### Body and Face Tracking

class ARBodyTrackingConfiguration

A configuration that tracks human body poses, planar surfaces, and images using the rear-facing camera.

