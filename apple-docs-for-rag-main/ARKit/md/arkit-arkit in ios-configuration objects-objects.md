

- ARKit
- ARKit in iOS
-  Configuration Objects 

API Collection

# Configuration Objects

Configure your augmented reality session to detect and track specific types of content.

## Overview

Configuration objects define how ARKit sets up and runs your augmented reality session. Although ARWorldTrackingConfiguration provides the widest range of features in a rear-camera experience, each feature consumes device energy and compute cycles. So to maximize device uptime and performance, enable additional options sparingly.

If another AR configuration fulfills your requirements with a more concise feature set, use that configuration instead. For example, use ARBodyTrackingConfiguration instead of a world-tracking configuration for 3D motion-capture if you don’t need user face-tracking, collaboration, or scene reconstruction.

### Select frame features

Some configurations support subfeatures that relate to a session’s frame. Enable these features by setting the following flags in the configuration’s frameSemantics:

bodyDetection  
Enables 2D human body tracking.

personSegmentation  
Enables people occlusion.

personSegmentationWithDepth  
Enables people occlusion based on whether the people in the camera feed are closer to the camera than the virtual content.

Use supportsFrameSemantics(_:) to verify whether the iOS device supports the ARConfiguration.FrameSemantics you desire before setting frameSemantics.

Important

To maximize device responsiveness, refrain from turning on people occlusion for single-user experiences when you don’t expect people in the scene.

### Switch configurations at runtime

To toggle features like plane detection, frame semantics, and environment texturing, you switch your configuration at runtime by calling runWithConfiguration: on your existing session. Where possible, ARKit maintains all the information collected during the session under the prior configuration, such as information about the physical environment and anchors.

Tip

You can gracefully downgrade the AR experience in the event of low-power or thermal events. For example, you could temporarily switch from a world-tracking configuration to a position-tracking configuration (ARPositionalTrackingConfiguration) if your app can function at a basic level in that limited capacity until the device cools down.

If your session switches between face- and world-tracking configurations, the session doesn’t maintain state.

### Enable high-quality video and custom capture settings

In iOS 16, you can enable a 4K and high dynamic range (HDR) video format. In addition, you can customize your session’s video settings through the underlying AV capture device.

To determine whether your session supports 4K, call recommendedVideoFormatFor4KResolution.

```
guard let hiResFormat = ARWorldTrackingConfiguration.recommendedVideoFormatFor4KResolution else {
   print("4K video format not supported."); return }
```

Then, create a configuration with the format. You can also indicate the intent to enable HDR by setting videoHDRAllowed to `true`.

```
var config = ARWorldTrackingConfiguration()
config.videoFormat = hiResFormat
config.videoHDRAllowed = true
session.run(config)
```

If the device supports a configurable capture session, the configurableCaptureDeviceForPrimaryCamera provides the underlying capture device that you can adjust as needed.

```
if let device = ARWorldTrackingConfiguration.configurableCaptureDeviceForPrimaryCamera {
   do { try device.lockForConfiguration()
      // Configure capture settings here.
      device.unlockForConfiguration()
   } catch { /* Error handling. */ }
}
```

### Capture high-resolution still frames

In iOS 16, you can enable high-resolution frame capture by calling recommendedVideoFormatForHighResolutionFrameCapturing on your configuration. If the device supports high-resolution stills, the function returns a video format you can use to start a session:

```
guard let hiResFormat = type(of: config).recommendedVideoFormatForHighResolutionFrameCapturing else {
    fatalError("The device doesn't support high-resolution stills.") }
config.videoFormat = hiResFormat
arSession.run(config)
```

During the session, capture a high-resolution still frame at any time by calling captureHighResolutionFrame(completion:):

```
arSession.captureHighResolutionFrame { (frame, error) in
    if let frame = frame {
        saveHiResFrame(frame)
    } else { /* Error handling. */ }
```

## Topics

### Common Configuration Details

class ARConfiguration

The base object that contains information about how to configure an augmented reality session.

### Spatial Tracking

Understanding World Tracking

Discover features and best practices for building rear-camera AR experiences.

class ARWorldTrackingConfiguration

A configuration that tracks the position of a device in relation to objects in the environment.

class ARGeoTrackingConfiguration

A configuration that tracks locations with GPS, map data, and a device’s compass.

class AROrientationTrackingConfiguration

A configuration that tracks only the device’s orientation using the rear-facing camera.

class ARPositionalTrackingConfiguration

A configuration that tracks only the device’s position in 3D space.

### Body and Face Tracking

class ARBodyTrackingConfiguration

A configuration that tracks human body poses, planar surfaces, and images using the rear-facing camera.

class ARFaceTrackingConfiguration

A configuration that tracks facial movement and expressions using the front camera.

### Image Recognition

class ARImageTrackingConfiguration

A configuration that tracks known images using the rear-facing camera.

### Object Detection

class ARObjectScanningConfiguration

A configuration that recognizes objects and collects high-fidelity data about specific objects using the rear-facing camera.

## See Also

### Setup

Choosing Which Camera Feed to Augment

Add visual effects to the user’s environment in an AR experience through the front or rear camera.

Managing Session Life Cycle and Tracking Quality

Keep the user informed on the current session state and recover from interruptions.

Displaying an AR Experience with Metal

Control rendering of your app’s virtual content on top of a camera feed.

class ARSession

The object that manages the major tasks associated with every AR experience, such as motion tracking, camera passthrough, and image analysis.

