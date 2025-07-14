

- Metal
- MTLPipelineOption
-  argumentInfo Deprecated

Type Property

# argumentInfo

An option instance that provides argument information for textures and threadgroup memory.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
static var argumentInfo: MTLPipelineOption { get }
```

## Discussion

This option provides all properties of a MTLArgument object, except for bufferStructType and bufferPointerType, which are `nil`. To obtain these detailed buffer type properties, retrieve the bufferTypeInfo instance.

## See Also

### Retrieving Argument Information

static var bufferTypeInfo: MTLPipelineOption

An option instance that provides detailed buffer type information for buffer arguments.

static var failOnBinaryArchiveMiss: MTLPipelineOption

An option that specifies that Metal only creates the pipeline state object if the compiled shader is present inside a linked binary archive.

