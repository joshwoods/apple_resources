

- ARKit
-  ARDepthData 

Class

# ARDepthData

An object that describes the distance to regions of the real world from the plane of the camera.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class ARDepthData
```

## Overview

This object contains the following depth information that the LiDAR scanner captures at runtime:

- Every pixel in the depthMap maps to a region of the visible scene (capturedImage), where the pixel value defines that region’s distance from the plane of the camera in meters.

- The confidenceMap property measures the accuracy of the corresponding depth data in depthMap, and is useful in filtering out lower-accuracy depth values if an app’s algorithm required it.

ARWorldTrackingConfiguration exposes this depth information in the sceneDepth property which it updates every frame. To enable scene depth, add the sceneDepth frame semantic to a world-tracking configuration’s frameSemantics and frames vended by the session contain ARDepthData captured by the LiDAR scanner.

## Topics

### Depth Information

var depthMap: CVPixelBuffer

The estimated distance from the device to its environment, in meters.

var confidenceMap: CVPixelBuffer?

The framework’s confidence in the accuracy of the depth-map data.

enum ARConfidenceLevel

Degrees to which the framework is confident about depth-data accuracy.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Video Frame Analysis

Displaying a point cloud using scene depth

Present a visualization of the physical environment by placing points based a scene’s depth data.

Creating a fog effect using scene depth

Apply virtual fog to the physical environment.

class ARFrame

A video image captured as part of a session with position-tracking information.

class ARPointCloud

A collection of points in the world coordinate space of the AR session.

