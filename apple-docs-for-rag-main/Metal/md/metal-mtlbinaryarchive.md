

- Metal
-  MTLBinaryArchive 

Protocol

# MTLBinaryArchive

A container for pipeline state descriptors and their associated compiled shader code.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
protocol MTLBinaryArchive : NSObjectProtocol
```

## Mentioned in 

Creating Binary Archives from Device-Built Pipeline State Objects

## Topics

### Identifying the Archive

var device: any MTLDevice

The Metal device object that created the binary archive.

**Required**

var label: String?

A string that identifies the library.

**Required**

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

func addFunction(descriptor: MTLFunctionDescriptor, library: any MTLLibrary) throws

Adds a description of a function to the archive.

**Required**

### Serializing Archives

func serialize(to: URL) throws

Writes the contents of the archive to a file.

**Required**

### Instance Methods

func addLibrary(descriptor: MTLStitchedLibraryDescriptor) throws

**Required**

func addMeshRenderPipelineFunctions(descriptor: MTLMeshRenderPipelineDescriptor) throws

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Shader Library Management

protocol MTLLibrary

A collection of Metal shader functions.

protocol MTLDynamicLibrary

A dynamically linkable representation of compiled shader code for a specific Metal device object.

class MTLCompileOptions

Compilation settings for a Metal shader library.

enum MTLLibraryType

A set of options for Metal library types.

enum MTLLanguageVersion

Metal shading language versions.

enum MTLCompileSymbolVisibility

enum MTLLibraryOptimizationLevel

The optimization options for the Metal compiler.

