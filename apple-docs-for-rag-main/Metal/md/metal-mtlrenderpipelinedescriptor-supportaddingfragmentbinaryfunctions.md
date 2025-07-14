

- Metal
- MTLRenderPipelineDescriptor
-  supportAddingFragmentBinaryFunctions 

Instance Property

# supportAddingFragmentBinaryFunctions

A Boolean value that indicates whether you can use the pipeline to create new pipelines by adding binary functions to the fragment shader’s callable functions list.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var supportAddingFragmentBinaryFunctions: Bool { get set }
```

## See Also

### Specifying Precompiled Shader Binaries

var supportAddingVertexBinaryFunctions: Bool

A Boolean value that indicates whether you can use the pipeline to create new pipelines by adding binary functions to the vertex shader’s callable functions list.

var binaryArchives: [any MTLBinaryArchive]?

An array of binary archives to search for precompiled versions of the shader.

