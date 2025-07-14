

- ARKit
- ARFrame
-  estimatedDepthData 

Instance Property

# estimatedDepthData

A buffer that represents the estimated depth values from the camera feed that you use to occlude virtual content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var estimatedDepthData: CVPixelBuffer? { get }
```

## Discussion

Each non-background pixel in the segmentation buffer maps to a depth value in this buffer. Use this to occlude people from the rendering of your app’s virtual content.

If you implement a custom renderer, you apply this property by using alpha and depth mattes provided with ARMatteGenerator.

Apps using one of the standard renderers don’t need this property to occlude virtual content with people. The standard renderers (ARView, ARSCNView, and ARSKView) enable people occlusion when you add personSegmentation or personSegmentationWithDepth to your configuration’s frameSemantics.

## See Also

### Checking for people

var detectedBody: ARBody2D?

The screen position information of a body that ARKit recognizes in the camera image.

class ARBody2D

The screen-space representation of a person ARKit recognizes in the camera feed.

var segmentationBuffer: CVPixelBuffer?

A buffer that contains pixel information identifying the shape of objects from the camera feed that you use to occlude virtual content.

enum SegmentationClass

A categorization of a pixel that defines a type of content you use to occlude your app’s virtual content.

