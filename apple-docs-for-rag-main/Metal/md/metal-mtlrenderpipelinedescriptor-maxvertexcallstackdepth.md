

- Metal
- MTLRenderPipelineDescriptor
-  maxVertexCallStackDepth 

Instance Property

# maxVertexCallStackDepth

The maximum function call depth from the top-most vertex shader function.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var maxVertexCallStackDepth: Int { get set }
```

## Discussion

The default value is 1.

## See Also

### Specifying Graphics Functions and Associated Data

var vertexFunction: (any MTLFunction)?

The vertex function the pipeline calls to process vertices.

var fragmentFunction: (any MTLFunction)?

The fragment function the pipeline calls to process fragments.

var maxFragmentCallStackDepth: Int

The maximum function call depth from the top-most fragment shader function.

