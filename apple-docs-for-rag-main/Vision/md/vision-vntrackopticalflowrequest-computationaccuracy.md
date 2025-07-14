

- Vision
- VNTrackOpticalFlowRequest
-  computationAccuracy 

Instance Property

# computationAccuracy

The level of accuracy to compute the optical flow.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var computationAccuracy: VNTrackOpticalFlowRequest.ComputationAccuracy { get set }
```

## Discussion

The computational time trends with accuracy level. The default value is VNTrackOpticalFlowRequest.ComputationAccuracy.medium.

## See Also

### Configuring the Request

enum ComputationAccuracy

Computational accuracy options.

var keepNetworkOutput: Bool

A Boolean value that indicates the raw pixel buffer continues to emit from the network.

var outputPixelFormat: OSType

The pixel format type of the output value.

