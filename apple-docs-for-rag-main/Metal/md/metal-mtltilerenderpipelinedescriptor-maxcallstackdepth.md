

- Metal
- MTLTileRenderPipelineDescriptor
-  maxCallStackDepth 

Instance Property

# maxCallStackDepth

The maximum function call depth from the top-most shader function.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var maxCallStackDepth: Int { get set }
```

## Discussion

The default value is 1.

## See Also

### Specifying Graphics Functions and Associated Data

var tileFunction: any MTLFunction

The compute kernel or fragment function the pipeline calls.

var tileBuffers: MTLPipelineBufferDescriptorArray

An array that contains the buffer mutability options for a render pipeline’s tile function.

