

- ARKit
-  ARFrame 

Class

# ARFrame

A video image captured as part of a session with position-tracking information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class ARFrame
```

## Mentioned in 

Displaying an AR Experience with Metal

## Overview

A running session continuously captures video frames from the device’s camera while ARKit analyzes the captures to determine the user’s position in the world. ARKit can provide this information to you in the form of an ARFrame in two ways:

- Occasionally, by accessing an ARSession object’s currentFrame

- Constantly, as a stream of frames through the session(_:didUpdate:) callback

To automatically receive all frames as ARKit captures them, make one of your objects the delegate of your app’s ARSession.

Each frame can contain additional data, for example, EXIF (exifData), or data based on any particular frameSemantics that you enable.

## Topics

### Accessing camera data

var camera: ARCamera

Information about the camera position, orientation, and imaging parameters used to capture the frame.

var capturedImage: CVPixelBuffer

A pixel buffer containing the image captured by the camera.

var timestamp: TimeInterval

The time at which the frame was captured.

var cameraGrainIntensity: Float

A value that specifies the amount of grain present in the camera grain texture.

var cameraGrainTexture: (any MTLTexture)?

A tileable Metal texture created by ARKit to match the visual characteristics of the current video stream.

var exifData: [String : Any]

Auxiliary data for the captured image.

### Accessing scene data

var lightEstimate: ARLightEstimate?

An estimate of lighting conditions based on the camera image.

func displayTransform(for: UIInterfaceOrientation, viewportSize: CGSize) -> CGAffineTransform

Returns an affine transform for converting between normalized image coordinates and a coordinate space appropriate for rendering the camera image onscreen.

var rawFeaturePoints: ARPointCloud?

The current intermediate results of the scene analysis ARKit uses to perform world tracking.

var capturedDepthData: AVDepthData?

Depth data captured in front-camera experiences.

var capturedDepthDataTimestamp: TimeInterval

The time at which depth data for the frame (if any) was captured.

var sceneDepth: ARDepthData?

Data on the distance between a device’s rear camera and real-world objects in an AR experience.

var smoothedSceneDepth: ARDepthData?

An average of distance measurements between a device’s rear camera and real-world objects that creates smoother visuals in an AR experience.

### Tracking and interacting with the real world

var anchors: [ARAnchor]

The list of anchors representing positions tracked or objects detected in the scene.

func raycastQuery(from: CGPoint, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment) -> ARRaycastQuery

Get a ray-cast query for a screen point.

func hitTest(CGPoint, types: ARHitTestResult.ResultType) -> [ARHitTestResult]

Searches for real-world objects or AR anchors in the captured camera image.

Deprecated

### Checking world-mapping status

var worldMappingStatus: ARFrame.WorldMappingStatus

The feasibility of generating or relocalizing a world map for this frame.

enum WorldMappingStatus

A value describing the world mapping status for the area visible in a given frame.

### Checking for people

var detectedBody: ARBody2D?

The screen position information of a body that ARKit recognizes in the camera image.

class ARBody2D

The screen-space representation of a person ARKit recognizes in the camera feed.

var segmentationBuffer: CVPixelBuffer?

A buffer that contains pixel information identifying the shape of objects from the camera feed that you use to occlude virtual content.

var estimatedDepthData: CVPixelBuffer?

A buffer that represents the estimated depth values from the camera feed that you use to occlude virtual content.

enum SegmentationClass

A categorization of a pixel that defines a type of content you use to occlude your app’s virtual content.

### Assessing geo-tracking condition

var geoTrackingStatus: ARGeoTrackingStatus?

The session’s condition with respect to geographic tracking at the time the session captured the frame.

class ARGeoTrackingStatus

The state, accuracy, and reason that are possible for geo-tracking’s current condition.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Accessing the camera frame

var currentFrame: ARFrame?

The most recent still frame captured by the active camera feed, including ARKit’s interpretation of it.

func captureHighResolutionFrame(completion: (ARFrame?, (any Error)?) -> Void)

Requests a frame outside of the normal frequency that contains a high-resolution captured image.

