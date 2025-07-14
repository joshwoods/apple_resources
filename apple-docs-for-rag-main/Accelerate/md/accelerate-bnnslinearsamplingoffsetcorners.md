

- Accelerate
-  BNNSLinearSamplingOffsetCorners 

Global Variable

# BNNSLinearSamplingOffsetCorners

The offset corners sampling mode.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var BNNSLinearSamplingOffsetCorners: BNNSLinearSamplingMode { get }
```

## Discussion

Given an input grid with a size of `Xin` and an output grid with a size `Xout`, this mode samples the grid using the following:

```
delta = max(1, Xin - 1) / Xout
spacing = ((Xout - 1) * delta) / (Xout - 1)

grid_point[i] = min(Xin-1, max(0, 0.5*delta + i*spacing)), for i=0,1,...,Xout-1
```

## See Also

### Constants

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSLinearSamplingDefault: BNNSLinearSamplingMode

The default linear sampling mode.

var BNNSLinearSamplingAlignCorners: BNNSLinearSamplingMode

The align corners sampling mode.

var BNNSLinearSamplingUnalignCorners: BNNSLinearSamplingMode

The unalign corners sampling mode.

var BNNSLinearSamplingStrictAlignCorners: BNNSLinearSamplingMode

The strict align corners sampling mode.

