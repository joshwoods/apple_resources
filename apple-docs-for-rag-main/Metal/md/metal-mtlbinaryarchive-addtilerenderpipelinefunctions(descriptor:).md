

- Metal
- MTLBinaryArchive
-  addTileRenderPipelineFunctions(descriptor:) 

Instance Method

# addTileRenderPipelineFunctions(descriptor:)

Adds a description of a tile renderer pipeline to the archive.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func addTileRenderPipelineFunctions(descriptor: MTLTileRenderPipelineDescriptor) throws
```

**Required**

## Parameters 

`descriptor`  

A description of the tile renderer pipeline to archive.

## See Also

### Adding Pipeline Descriptors

func addComputePipelineFunctions(descriptor: MTLComputePipelineDescriptor) throws

Adds a description of a compute pipeline to the archive.

**Required**

func addRenderPipelineFunctions(descriptor: MTLRenderPipelineDescriptor) throws

Adds a description of a render pipeline to the archive.

**Required**

func addFunction(descriptor: MTLFunctionDescriptor, library: any MTLLibrary) throws

Adds a description of a function to the archive.

**Required**

