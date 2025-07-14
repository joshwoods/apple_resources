

- Metal
- MTLPipelineOption
-  failOnBinaryArchiveMiss 

Type Property

# failOnBinaryArchiveMiss

An option that specifies that Metal only creates the pipeline state object if the compiled shader is present inside a linked binary archive.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
static var failOnBinaryArchiveMiss: MTLPipelineOption { get }
```

## Mentioned in 

Creating Binary Archives from Device-Built Pipeline State Objects

## Discussion

When this value is `true` and a compiled shader isn’t available, Metal produces an error rather than attempting to recompile on-demand on the GPU.

## See Also

### Retrieving Argument Information

static var bufferTypeInfo: MTLPipelineOption

An option instance that provides detailed buffer type information for buffer arguments.

static var argumentInfo: MTLPipelineOption

An option instance that provides argument information for textures and threadgroup memory.

Deprecated

