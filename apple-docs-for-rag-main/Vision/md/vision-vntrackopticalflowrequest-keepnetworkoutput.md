

- Vision
- VNTrackOpticalFlowRequest
-  keepNetworkOutput 

Instance Property

# keepNetworkOutput

A Boolean value that indicates the raw pixel buffer continues to emit from the network.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var keepNetworkOutput: Bool { get set }
```

## Discussion

The default value is false; otherwise, the request ignores outputPixelFormat.

## See Also

### Configuring the Request

var computationAccuracy: VNTrackOpticalFlowRequest.ComputationAccuracy

The level of accuracy to compute the optical flow.

enum ComputationAccuracy

Computational accuracy options.

var outputPixelFormat: OSType

The pixel format type of the output value.

