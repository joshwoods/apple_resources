

- Metal Performance Shaders Graph
- MPSGraphRandomOpDescriptor
-  samplingMethod 

Instance Property

# samplingMethod

The sampling method of the distribution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var samplingMethod: MPSGraphRandomNormalSamplingMethod { get set }
```

## Discussion

This value is used for Normal and Truncated Normal disributions. See MPSGraphRandomNormalSamplingMethod. Defaults to MPSGraphRandomNormalSamplingInvCDF.

