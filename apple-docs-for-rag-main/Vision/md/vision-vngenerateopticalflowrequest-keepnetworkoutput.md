

- Vision
- VNGenerateOpticalFlowRequest
-  keepNetworkOutput 

Instance Property

# keepNetworkOutput

A Boolean value that indicates whether to keep the raw pixel buffer coming from the machine learning network.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var keepNetworkOutput: Bool { get set }
```

## Discussion

The default is false. When you set this to true, the system ignores outputPixelFormat. Setting this for revision 1 has no effect because it’s not machine learning-based.

## See Also

### Configuring the Request

var computationAccuracy: VNGenerateOpticalFlowRequest.ComputationAccuracy

The accuracy level for computing optical flow.

enum ComputationAccuracy

The supported optical flow accuracy levels.

var outputPixelFormat: OSType

The output buffer’s pixel format.

