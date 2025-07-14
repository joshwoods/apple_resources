

- ARKit
-  ARBodyTrackingConfiguration 

Class

# ARBodyTrackingConfiguration

A configuration that tracks human body poses, planar surfaces, and images using the rear-facing camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARBodyTrackingConfiguration
```

## Overview

When ARKit identifies a person in the rear camera’s feed, it calls session(_:didAdd:), passing an ARBodyAnchor you can use to track the body’s movement.

When you enable plane detection and image detection, you can use a body anchor to display a virtual character and set the character on a surface or image that you choose.

By default, frameSemantics includes bodyDetection, which gives you access to the joint positions of a person that ARKit detects in the camera feed via the frame’s detectedBody.

## Topics

### Creating a Configuration

init()

Creates a new body tracking configuration.

var initialWorldMap: ARWorldMap?

The state from a previous AR session to attempt to resume with this session configuration.

### Estimating Body Scale

var automaticSkeletonScaleEstimationEnabled: Bool

A flag that determines whether ARKit estimates the height of a body that it’s tracking.

### Enabling Auto Focus

var isAutoFocusEnabled: Bool

A Boolean value that determines whether the device camera uses fixed focus or autofocus behavior.

### Enabling Plane Detection

var planeDetection: ARWorldTrackingConfiguration.PlaneDetection

A value specifying whether and how the session attempts to automatically detect flat surfaces in the camera-captured image.

struct PlaneDetection

Options for whether and how the framework detects flat surfaces in captured images.

### Enabling Image Tracking

var automaticImageScaleEstimationEnabled: Bool

A flag that instructs ARKit to estimate and set the scale of a tracked image on your behalf.

var detectionImages: Set&lt;ARReferenceImage>

A set of images that ARKit searches for in the user’s environment.

var maximumNumberOfTrackedImages: Int

The number of image anchors to monitor closely for position and orientation updates.

### Adding Realistic Reflections

var wantsHDREnvironmentTextures: Bool

A flag that instructs ARKit to create environment textures in HDR format.

var environmentTexturing: ARWorldTrackingConfiguration.EnvironmentTexturing

The behavior ARKit uses for generating environment textures.

### Accessing App Clip Codes

Interacting with App Clip Codes in AR

Display content and provide services in an AR experience with App Clip Codes.

class var supportsAppClipCodeTracking: Bool

A flag that indicates if the device tracks App Clip Codes.

var appClipCodeTrackingEnabled: Bool

A Boolean value that indicates if the framework searches the physical environment for App Clip Codes.

class ARAppClipCodeAnchor

An anchor that tracks the position and orientation of an App Clip Code in the physical environment.

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

class ARFaceTrackingConfiguration

A configuration that tracks facial movement and expressions using the front camera.

