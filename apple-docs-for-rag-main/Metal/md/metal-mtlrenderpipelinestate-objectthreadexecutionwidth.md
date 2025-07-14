

- Metal
- MTLRenderPipelineState
-  objectThreadExecutionWidth 

Instance Property

# objectThreadExecutionWidth

The number of threads the render pass applies to a SIMD group for an object shader.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var objectThreadExecutionWidth: Int { get }
```

**Required**

## Discussion

You can access the value of this property in your shader code by adding an integer parameter with the `[[threads_per_simdgroup]]` attribute. For more information about this attribute, see the Metal Shading Language Specification (PDF).

## See Also

### Checking Object Shader Memory Requirements

var maxTotalThreadsPerObjectThreadgroup: Int

The largest number of threads the pipeline state can have in a single object shader threadgroup.

**Required**

