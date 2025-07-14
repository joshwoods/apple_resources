

- Metal
- MTLRenderPipelineDescriptor
-  vertexFunction 

Instance Property

# vertexFunction

The vertex function the pipeline calls to process vertices.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var vertexFunction: (any MTLFunction)? { get set }
```

## Discussion

The default value is `nil`. The vertex function must always be specified. The vertex function can be either a regular vertex function or a post-tessellation vertex function.

## See Also

### Specifying Graphics Functions and Associated Data

var fragmentFunction: (any MTLFunction)?

The fragment function the pipeline calls to process fragments.

var maxVertexCallStackDepth: Int

The maximum function call depth from the top-most vertex shader function.

var maxFragmentCallStackDepth: Int

The maximum function call depth from the top-most fragment shader function.

