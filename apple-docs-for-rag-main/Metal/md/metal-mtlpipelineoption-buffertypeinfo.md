

- Metal
- MTLPipelineOption
-  bufferTypeInfo 

Type Property

# bufferTypeInfo

An option instance that provides detailed buffer type information for buffer arguments.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
static var bufferTypeInfo: MTLPipelineOption { get }
```

## Discussion

This option provides the bufferStructType and bufferPointerType properties for the MTLPipelineOption stored in argumentInfo.

## See Also

### Retrieving Argument Information

static var failOnBinaryArchiveMiss: MTLPipelineOption

An option that specifies that Metal only creates the pipeline state object if the compiled shader is present inside a linked binary archive.

static var argumentInfo: MTLPipelineOption

An option instance that provides argument information for textures and threadgroup memory.

Deprecated

