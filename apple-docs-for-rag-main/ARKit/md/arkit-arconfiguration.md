

- ARKit
-  ARConfiguration 

Class

# ARConfiguration

The base object that contains information about how to configure an augmented reality session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARConfiguration
```

## Mentioned in 

Verifying Device Support and User Permission

## Overview

ARConfiguration defines a base class for the different options you can configure in your AR experience.

All AR configurations establish a correspondence between the real world that the device inhabits and the virtual 3D-coordinate space, where you model content. When your app mixes virtual content with a live-camera image, the user experiences the illusion that your virtual content is part of the real world.

To acquire the live-camera imagery, ARKit manages a camera-capture pipeline for you. Depending on the configuration you choose, it determines the cameras that capture imagery, and which camera feed the app displays.

AR apps recognize real-world regions of interest. At runtime, ARKit generates an ARAnchor for a real-world object it recognizes, which allows an app to refer to its details, such as size and physical location. The configuration you choose determines the kinds of real-world objects ARKit recognizes and makes available to your app.

Don’t allocate ARConfiguration yourself; instead, instantiate one of its subclasses.

For more information about the camera-capture pipeline, see Choosing Which Camera Feed to Augment.

## Topics

### Verifying device support

class var isSupported: Bool

A Boolean value indicating whether the current device supports this session configuration class.

### Enabling frame features

var frameSemantics: ARConfiguration.FrameSemantics

The set of active semantics on the frame.

struct FrameSemantics

Types of optional frame features you can enable in your app.

class func supportsFrameSemantics(ARConfiguration.FrameSemantics) -> Bool

Checks whether a particular feature is supported.

### Configuring the AR session

var isLightEstimationEnabled: Bool

A Boolean value specifying whether ARKit analyzes scene lighting in captured camera images.

var worldAlignment: ARConfiguration.WorldAlignment

A value specifying how the session maps real-world device motion into a 3D scene coordinate system.

enum WorldAlignment

Options for how ARKit constructs a scene coordinate system based on real-world device motion.

### Managing video capture options

var videoFormat: ARConfiguration.VideoFormat

Video format of the session output.

class var supportedVideoFormats: [ARConfiguration.VideoFormat]

The set of video capture formats available on the current device.

class VideoFormat

A video size and frame rate specification for use with an AR session.

var videoHDRAllowed: Bool

Enables high dynamic range (HDR) for the session’s camera feed.

class var configurableCaptureDeviceForPrimaryCamera: AVCaptureDevice?

An object that enables you to alter the appearance of a frame’s captured image.

class var recommendedVideoFormatFor4KResolution: ARConfiguration.VideoFormat?

Provides a 4K video format if the device and configuration support it.

class var recommendedVideoFormatForHighResolutionFrameCapturing: ARConfiguration.VideoFormat?

Returns a video format that the framework recommends for high-resolution-still-image capture.

### Recording Audio

var providesAudioData: Bool

A Boolean value that specifies whether to capture audio during the AR session.

### Reconstructing the Scene

struct SceneReconstruction

Options that enable ARKit to detect the shape of the physical environment.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ARBodyTrackingConfiguration
- ARFaceTrackingConfiguration
- ARGeoTrackingConfiguration
- ARImageTrackingConfiguration
- ARObjectScanningConfiguration
- AROrientationTrackingConfiguration
- ARPositionalTrackingConfiguration
- ARWorldTrackingConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

