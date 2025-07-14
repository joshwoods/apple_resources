

- Metal
- MTLBinaryArchive
-  addFunction(descriptor:library:) 

Instance Method

# addFunction(descriptor:library:)

Adds a description of a function to the archive.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func addFunction(
    descriptor: MTLFunctionDescriptor,
    library: any MTLLibrary
) throws
```

**Required**

## Parameters 

`descriptor`  

`library`  

## See Also

### Adding Pipeline Descriptors

func addComputePipelineFunctions(descriptor: MTLComputePipelineDescriptor) throws

Adds a description of a compute pipeline to the archive.

**Required**

func addRenderPipelineFunctions(descriptor: MTLRenderPipelineDescriptor) throws

Adds a description of a render pipeline to the archive.

**Required**

func addTileRenderPipelineFunctions(descriptor: MTLTileRenderPipelineDescriptor) throws

Adds a description of a tile renderer pipeline to the archive.

**Required**

