

- ARKit
-  ARWorldTrackingConfiguration 

Class

# ARWorldTrackingConfiguration

A configuration that tracks the position of a device in relation to objects in the environment.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARWorldTrackingConfiguration
```

## Mentioned in 

Choosing Which Camera Feed to Augment

## Overview

The ARWorldTrackingConfiguration class tracks the device’s movement with six degrees of freedom (6DOF): the three rotation axes (roll, pitch, and yaw), and three translation axes (movement in x, y, and z).

This kind of tracking can create immersive AR experiences: A virtual object can appear to stay in the same place relative to the real world, even as the user tilts the device to look above or below the object, or moves the device around to see the object’s sides and back.

World-tracking sessions also provide several ways for your app to recognize or interact with elements of the real-world scene visible to the camera:

- Find real-world horizontal or vertical surfaces with planeDetection. Add the surfaces to the session as ARPlaneAnchor objects.

- Recognize and track the movement of 2D images with detectionImages. Add 2D images to the scene as ARImageAnchor objects.

- Recognize 3D objects with detectionObjects. Add 3D objects to the scene as ARObjectAnchor objects.

- Find the 3D positions of real-world features that correspond to a touch point on the device’s screen with ray casting.

## Topics

### Creating a Configuration

init()

Initializes a new world-tracking configuration.

var initialWorldMap: ARWorldMap?

The state from a previous AR session to attempt to resume with this session configuration.

### Tracking Surfaces

var planeDetection: ARWorldTrackingConfiguration.PlaneDetection

The configuration’s plane detection options.

struct PlaneDetection

Options for whether and how the framework detects flat surfaces in captured images.

var sceneReconstruction: ARConfiguration.SceneReconstruction

A flag that enables scene reconstruction.

class func supportsSceneReconstruction(ARConfiguration.SceneReconstruction) -> Bool

Checks if the device supports scene reconstruction.

### Detecting or Tracking Images

var detectionImages: Set&lt;ARReferenceImage>!

A set of images that ARKit searches for in the user’s environment.

var maximumNumberOfTrackedImages: Int

The number of image anchors to monitor closely for position and orientation updates.

var automaticImageScaleEstimationEnabled: Bool

A flag that instructs the framework to estimate and set the scale of a detected or tracked image on your behalf.

### Detecting 3D Objects

var detectionObjects: Set&lt;ARReferenceObject>

A set of 3D objects that the framework attempts to detect in the user’s environment.

### Tracking the User’s Face

var userFaceTrackingEnabled: Bool

A flag that determines whether ARKit tracks the user’s face in a world-tracking session.

class var supportsUserFaceTracking: Bool

A Boolean value that tells you whether the iOS device supports tracking the user’s face during a world-tracking session.

### Creating Realistic Reflections

var environmentTexturing: ARWorldTrackingConfiguration.EnvironmentTexturing

An option that determines how the framework generates environment textures.

enum EnvironmentTexturing

The available environment texturing options for world tracking.

class AREnvironmentProbeAnchor

An object that provides environmental lighting information for a specific area of space in a world-tracking AR session.

var wantsHDREnvironmentTextures: Bool

A flag that instructs the framework to create environment textures in HDR format.

### Managing Device Camera Behavior

var isAutoFocusEnabled: Bool

A Boolean value that determines whether the device camera uses fixed focus or autofocus behavior.

### Enabling Collaboration

var isCollaborationEnabled: Bool

A flag that opts you in to a peer-to-peer multiuser AR experience.

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

### Spatial Tracking

Understanding World Tracking

Discover features and best practices for building rear-camera AR experiences.

class ARGeoTrackingConfiguration

A configuration that tracks locations with GPS, map data, and a device’s compass.

class AROrientationTrackingConfiguration

A configuration that tracks only the device’s orientation using the rear-facing camera.

class ARPositionalTrackingConfiguration

A configuration that tracks only the device’s position in 3D space.

