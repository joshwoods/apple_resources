

- Accelerate
-  BNNSShuffleTypeSpaceToDepthNCHW 

Global Variable

# BNNSShuffleTypeSpaceToDepthNCHW

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
var BNNSShuffleTypeSpaceToDepthNCHW: BNNSShuffleType { get }
```

## See Also

### Constants

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSShuffleTypePixelShuffleNCHW: BNNSShuffleType

The pixel shuffle for the NCHW (batch, channels, height, width) format, equivalent to depth-to-space in Column Row Depth (CRD) mode.

var BNNSShuffleTypePixelUnshuffleNCHW: BNNSShuffleType

The pixel unshuffle for the NCHW (batch, channels, height, width) format, equivalent to space-to-depth in Column Row Depth (CRD) mode.

var BNNSShuffleTypeDepthToSpaceNCHW: BNNSShuffleType

