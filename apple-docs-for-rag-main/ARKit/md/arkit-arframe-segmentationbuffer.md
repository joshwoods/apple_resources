

- ARKit
- ARFrame
-  segmentationBuffer 

Instance Property

# segmentationBuffer

A buffer that contains pixel information identifying the shape of objects from the camera feed that you use to occlude virtual content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var segmentationBuffer: CVPixelBuffer? { get }
```

## Discussion

ARKit generates the contents of this buffer by processing the camera feed.

If you implement a custom renderer, you apply this property by using alpha and depth mattes provided with ARMatteGenerator.

Apps using one of the standard renderers don’t need this this property to occlude virtual content with people. The standard renderers (ARView, ARSCNView, and ARSKView) enable people occlusion when you add personSegmentation or personSegmentationWithDepth to your configuration’s frameSemantics.

## See Also

### Checking for people

var detectedBody: ARBody2D?

The screen position information of a body that ARKit recognizes in the camera image.

class ARBody2D

The screen-space representation of a person ARKit recognizes in the camera feed.

var estimatedDepthData: CVPixelBuffer?

A buffer that represents the estimated depth values from the camera feed that you use to occlude virtual content.

enum SegmentationClass

A categorization of a pixel that defines a type of content you use to occlude your app’s virtual content.

