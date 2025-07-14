

- ARKit
-  ARBody2D 

Class

# ARBody2D

The screen-space representation of a person ARKit recognizes in the camera feed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARBody2D
```

## Overview

When ARKit recognizes a person in the camera feed, it estimates the screen-space location of the body’s joints and provides the location to you through current frame’s detectedBody.

## Topics

### Getting Joint Information

var skeleton: ARSkeleton2D

An object that contains the screen position of a body’s joints.

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

### Checking for people

var detectedBody: ARBody2D?

The screen position information of a body that ARKit recognizes in the camera image.

var segmentationBuffer: CVPixelBuffer?

A buffer that contains pixel information identifying the shape of objects from the camera feed that you use to occlude virtual content.

var estimatedDepthData: CVPixelBuffer?

A buffer that represents the estimated depth values from the camera feed that you use to occlude virtual content.

enum SegmentationClass

A categorization of a pixel that defines a type of content you use to occlude your app’s virtual content.

