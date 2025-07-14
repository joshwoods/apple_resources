

- Metal
- MTLTileRenderPipelineDescriptor
-  tileBuffers 

Instance Property

# tileBuffers

An array that contains the buffer mutability options for a render pipeline’s tile function.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 11.0+visionOS 1.0+

``` source
var tileBuffers: MTLPipelineBufferDescriptorArray { get }
```

## Discussion

This property returns an array of MTLPipelineBufferDescriptor objects, with each array index corresponding to the same index in the buffer argument table for the render pipeline’s tile shader.

## See Also

### Specifying Graphics Functions and Associated Data

var tileFunction: any MTLFunction

The compute kernel or fragment function the pipeline calls.

var maxCallStackDepth: Int

The maximum function call depth from the top-most shader function.

