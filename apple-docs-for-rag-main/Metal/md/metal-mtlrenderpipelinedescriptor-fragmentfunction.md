

- Metal
- MTLRenderPipelineDescriptor
-  fragmentFunction 

Instance Property

# fragmentFunction

The fragment function the pipeline calls to process fragments.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var fragmentFunction: (any MTLFunction)? { get set }
```

## Discussion

The default value is `nil`. If this value is `nil`, then there is no fragment function and therefore no writes to the color render target occur. Depth and stencil writes and visibility result counting can still proceed.

## See Also

### Specifying Graphics Functions and Associated Data

var vertexFunction: (any MTLFunction)?

The vertex function the pipeline calls to process vertices.

var maxVertexCallStackDepth: Int

The maximum function call depth from the top-most vertex shader function.

var maxFragmentCallStackDepth: Int

The maximum function call depth from the top-most fragment shader function.

