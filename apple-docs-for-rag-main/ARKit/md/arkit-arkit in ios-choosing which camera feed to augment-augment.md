

- ARKit
- ARKit in iOS
-  Choosing Which Camera Feed to Augment 

Article

# Choosing Which Camera Feed to Augment

Add visual effects to the user’s environment in an AR experience through the front or rear camera.

## Overview

iOS devices come equipped with multiple cameras, and for each ARKit session you need to choose which camera’s feed to augment. ARKit 3 and later provide simultaneous anchors from all cameras (see Combining user face-tracking and world tracking), but you still must choose one camera feed to show to the user at a time.

### Augmented Reality with the Rear Camera

The most common kinds of AR experience display a view from the device’s rear camera, augmented by other visual content, giving the user a new way to see and interact with the world around them.

ARWorldTrackingConfiguration provides this kind of experience: ARKit tracks the real-world the user inhabits, and matches it with a coordinate space for you to place virtual content. World tracking also offers features to make AR experiences more immersive, like the ability to recognize objects and images in the user’s environment and respond to real-world lighting conditions.

### Augmented Reality with the Front Camera

For iOS devices that have a TrueDepth camera, ARFaceTrackingConfiguration enables you to augment the front-camera feed, while providing you with real-time tracking for the pose and expression of faces. With that information, that you might, for example, choose to overlay realistic virtual masks. Or, you might omit the camera view and use facial expression data to animate virtual characters, as in the Animoji app for iMessage.

## See Also

### Setup

Managing Session Life Cycle and Tracking Quality

Keep the user informed on the current session state and recover from interruptions.

Displaying an AR Experience with Metal

Control rendering of your app’s virtual content on top of a camera feed.

class ARSession

The object that manages the major tasks associated with every AR experience, such as motion tracking, camera passthrough, and image analysis.

Configuration Objects

Configure your augmented reality session to detect and track specific types of content.

