

- ARKit
- ARFrame
-  ARFrame.SegmentationClass 

Enumeration

# ARFrame.SegmentationClass

A categorization of a pixel that defines a type of content you use to occlude your app’s virtual content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum SegmentationClass
```

## Overview

ARKit applies the categories defined in this class based on its interpretation of the camera feed’s pixel data. Only people are identified in a camera feed, and therefore the available pixel classifications are either ARFrame.SegmentationClass.person or ARFrame.SegmentationClass.none.

## Topics

### Classifying Pixels

case person

A classification of a pixel in the segmentation buffer as part of a person.

case none

A classification of a pixel in the segmentation buffer as unidentified.

### Initializers

init?(rawValue: UInt8)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking for people

var detectedBody: ARBody2D?

The screen position information of a body that ARKit recognizes in the camera image.

class ARBody2D

The screen-space representation of a person ARKit recognizes in the camera feed.

var segmentationBuffer: CVPixelBuffer?

A buffer that contains pixel information identifying the shape of objects from the camera feed that you use to occlude virtual content.

var estimatedDepthData: CVPixelBuffer?

A buffer that represents the estimated depth values from the camera feed that you use to occlude virtual content.

