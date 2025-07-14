

- ARKit
- ARFrame
-  detectedBody 

Instance Property

# detectedBody

The screen position information of a body that ARKit recognizes in the camera image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var detectedBody: ARBody2D? { get }
```

## Discussion

To enable 2D body detection, you add the bodyDetection frame semantic to your configuration’s frameSemantics property, or run your session with an ARBodyTrackingConfiguration, in which body detection is enabled by default.

## See Also

### Checking for people

class ARBody2D

The screen-space representation of a person ARKit recognizes in the camera feed.

var segmentationBuffer: CVPixelBuffer?

A buffer that contains pixel information identifying the shape of objects from the camera feed that you use to occlude virtual content.

var estimatedDepthData: CVPixelBuffer?

A buffer that represents the estimated depth values from the camera feed that you use to occlude virtual content.

enum SegmentationClass

A categorization of a pixel that defines a type of content you use to occlude your app’s virtual content.

