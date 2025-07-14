

- Metal Performance Shaders Graph
- MPSGraphRandomOpDescriptor
-  min 

Instance Property

# min

The lower range of the distribution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var min: Float { get set }
```

## Discussion

This value is used for Uniform distributions with float data types and Truncated Normal disributions. Defaults to 0 for uniform distributions and -2 for normal distributions.

