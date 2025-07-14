

- Metal
- MTLSamplerDescriptor
-  compareFunction 

Instance Property

# compareFunction

The sampler comparison function used when performing a sample compare operation on a depth texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var compareFunction: MTLCompareFunction { get set }
```

## Discussion

The default value is MTLCompareFunction.never.

The MTLFeatureSet.iOS_GPUFamily3_v1 and MTLFeatureSet.iOS_GPUFamily1_v1 feature sets allow you to define a framework-side sampler comparison function for a MTLSamplerState object. All feature sets support shader-side sampler comparison functions, as described in the Metal Shading Language Specification.

## See Also

### Declaring the Depth Comparison Mode

enum MTLCompareFunction

Options used to specify how a sample compare operation should be performed on a depth texture.

