

- Metal
- GPU Devices and Work Submission
- MTLDevice
-  Shader Library and Archive Creation 

API Collection

# Shader Library and Archive Creation

Create static and dynamic shader libraries, and binary shader archives.

## Topics

### Creating Shader Libraries

func makeDefaultLibrary() -> (any MTLLibrary)?

Creates a Metal library instance that contains the functions from your app’s default Metal library.

**Required**

func makeDefaultLibrary(bundle: Bundle) throws -> any MTLLibrary

Creates a Metal library instance that contains the functions in a bundle’s default Metal library.

**Required**

func makeLibrary(URL: URL) throws -> any MTLLibrary

Creates a Metal library instance that contains the functions in the Metal library file at a URL.

**Required**

func makeLibrary(source: String, options: MTLCompileOptions?) throws -> any MTLLibrary

Synchronously creates a Metal library instance by compiling the functions in a source string.

**Required**

func makeLibrary(source: String, options: MTLCompileOptions?, completionHandler: MTLNewLibraryCompletionHandler)

Asynchronously creates a Metal library instance by compiling the functions in a source string.

**Required**

func makeLibrary(stitchedDescriptor: MTLStitchedLibraryDescriptor) throws -> any MTLLibrary

Synchronously creates a Metal library from the function stitching graphs in a descriptor.

**Required**

func makeLibrary(stitchedDescriptor: MTLStitchedLibraryDescriptor, completionHandler: MTLNewLibraryCompletionHandler)

Asynchronously creates a Metal library from the function stitching graphs in a descriptor.

**Required**

func makeLibrary(data: DispatchData) throws -> any MTLLibrary

Creates a Metal library instance that contains the functions in a precompiled Metal library.

func makeLibrary(data: dispatch_data_t) throws -> any MTLLibrary

Creates a Metal library instance from a dispatch-data instance that contains the functions in a precompiled Metal library.

**Required** Default implementation provided.

typealias MTLNewLibraryCompletionHandler

A completion handler signature a method calls when it finishes creating a Metal library.

func makeLibrary(filepath: String) throws -> any MTLLibrary

Creates a Metal library instance that contains the functions in the Metal library file at a file path.

**Required**

Deprecated

### Creating Dynamic Shader Libraries

var supportsDynamicLibraries: Bool

A Boolean value that indicates whether the GPU device can create and use dynamic libraries in compute pipelines.

**Required**

var supportsRenderDynamicLibraries: Bool

A Boolean value that indicates whether the GPU device can create and use dynamic libraries in render pipelines.

**Required**

func makeDynamicLibrary(library: any MTLLibrary) throws -> any MTLDynamicLibrary

Creates a Metal dynamic library instance from a Metal library instance.

**Required**

func makeDynamicLibrary(url: URL) throws -> any MTLDynamicLibrary

Creates a Metal dynamic library instance that contains the functions in the Metal library file at a URL.

**Required**

enum Code

Error codes that Metal can generate when creating dynamic libraries.

let MTLDynamicLibraryDomain: String

The domain for Metal dynamic library errors.

### Creating Binary Shader Archives

func makeBinaryArchive(descriptor: MTLBinaryArchiveDescriptor) throws -> any MTLBinaryArchive

Creates a Metal binary archive instance.

**Required**

class MTLBinaryArchiveDescriptor

A description of a binary shader archive that you want to create.

enum Code

Error codes when creating binary archives of compiled shader code.

let MTLBinaryArchiveDomain: String

The domain for Metal binary archive errors.

## See Also

### Working with GPU Devices

Device Inspection

Locate and identify a GPU and the features it supports, and sample its counters.

Work Submission

Create queues that submit work to the GPU or load assets into GPU resources, and indirect command buffers that group your frequent commands together.

Pipeline State Creation

Create pipeline states for render and compute passes, samplers, depth and stencil states, and indirect command buffers.

Resource Creation

Load assets with input/output queues and make various resource instances, such as buffers, textures, acceleration structures, and memory heaps.

