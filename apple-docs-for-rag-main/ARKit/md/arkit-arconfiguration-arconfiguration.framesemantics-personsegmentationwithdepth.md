

- ARKit
- ARConfiguration
- ARConfiguration.FrameSemantics
-  personSegmentationWithDepth 

Type Property

# personSegmentationWithDepth

An option that indicates that people occlude your app’s virtual content depending on depth.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
static var personSegmentationWithDepth: ARConfiguration.FrameSemantics { get }
```

## Discussion

The personSegmentationWithDepth frame semantic specifies that any person ARKit detects in the camera feed should occlude virtual content, depending on the person’s depth in the scene.

When this option is enabled, ARKit sets the estimatedDepthData and segmentationBuffer properties to serve as a foundation for people occlusion. The standard renderers (ARView, and ARSCNView) use those properties to implement people occlusion for you. See frameSemantics for more information.

## See Also

### Occluding Virtual Content with People

static var personSegmentation: ARConfiguration.FrameSemantics

An option that indicates that people occlude your app’s virtual content.

