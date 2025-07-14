

- ARKit
- ARConfiguration
- ARConfiguration.FrameSemantics
-  bodyDetection 

Type Property

# bodyDetection

An option that indicates that 2D body detection is enabled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
static var bodyDetection: ARConfiguration.FrameSemantics { get }
```

## Discussion

When you set this option in your configuration’s frameSemantics property, ARKit describes the joint positions of a body it detects in the camera image, using normalized coordinates. See detectedBody for more information.

