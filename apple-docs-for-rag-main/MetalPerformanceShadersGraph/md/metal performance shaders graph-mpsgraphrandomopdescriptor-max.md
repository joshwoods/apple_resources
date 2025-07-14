

- Metal Performance Shaders Graph
- MPSGraphRandomOpDescriptor
-  max 

Instance Property

# max

The upper range of the distribution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var max: Float { get set }
```

## Discussion

This value is used for Uniform distributions with float data types and Truncated Normal disributions. Defaults to 1 for uniform distributions and 2 for normal distributions.

