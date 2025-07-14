

- Metal
-  Shader Libraries 

API Collection

# Shader Libraries

Manage and load your app’s Metal shaders.

## Overview

A Metal library represents a collection of one or more shaders. Xcode creates a library from the shader source files in a project, a Metal intermediate representation (IR) file, or a binary archive file. You can also create IR files from Metal source code by running the Metal compiler in a command-line environment.

Apps create the default library instance by calling a Metal device’s makeDefaultLibrary() method. The default library contains all the shaders from a project’s shader source files, which Xcode compiles at build time. Apps create additional libraries by passing an IR file to an MTLDevice instance’s makeLibrary(URL:) method or one of its sibling methods. The device can also create a library directly from source code by passing it as a string to the makeLibrary(source:options:) method. See Shader Library and Archive Creation for more information.

You can apply a shader from a library to a pipeline state’s entry point, such as the computeFunction property for a compute pass. Start by retrieving an MTLFunction instance from a library, which is a reference to the library’s shader, by calling its makeFunction(name:) method or a sibling method. Then set the function instance to the appropriate property of a pipeline descriptor. For example, an app can retrieve a vertex stage’s entry point shader from a library and assign it to the vertexFunction property of an MTLRenderPipelineDescriptor.

Dynamic libraries are a collection of other shaders, typically utility functions, that support the entry point shaders for a pipeline state. To create a dynamic library, pass an MTLLibrary instance to a device’s makeDynamicLibrary(library:) method, or pass a file URL to makeDynamicLibrary(url:). Add a dynamic library to a pipeline state by including it in an array of a pipeline descriptor’s preloaded libraries property. For example, if a vertex shader calls a shader in a dynamic library, directly or indirectly, add that dynamic library to the vertexPreloadedLibraries property’s array. You can also build dynamic libraries with the Metal compiler in Terminal.

Binary archives are precompiled static libraries for specific GPU architectures that allow you to avoid the cost of runtime shader compilation. Because Metal automatically builds and caches shaders on the device running an app, use binary archives as part of your distributed app, or deliver them through content updates. See Creating Binary Archives from Device-Built Pipeline State Objects for more information on how to build and distribute binary archives for any device that supports Metal.

## Topics

### Shader Compilation

Compile and manipulate Metal shader libraries from the command line.

Metal Libraries

Compile and manage Metal libraries from the command line.

Metal Dynamic Libraries

Create a single Metal library containing reusable code to reduce library size and avoid repeated shader compilation at runtime.

Metal Binary Archives

Distribute precompiled GPU-specific binaries as part of your app to avoid runtime compilation of Metal shaders.

### Shader Library Management

protocol MTLLibrary

A collection of Metal shader functions.

protocol MTLDynamicLibrary

A dynamically linkable representation of compiled shader code for a specific Metal device object.

protocol MTLBinaryArchive

A container for pipeline state descriptors and their associated compiled shader code.

class MTLCompileOptions

Compilation settings for a Metal shader library.

enum MTLLibraryType

A set of options for Metal library types.

enum MTLLanguageVersion

Metal shading language versions.

enum MTLCompileSymbolVisibility

enum MTLLibraryOptimizationLevel

The optimization options for the Metal compiler.

### Shader Functions

class MTLFunctionDescriptor

A description of a function object to create.

protocol MTLFunction

An object that represents a public shader function in a Metal library.

protocol MTLFunctionHandle

An object representing a function that you can add to a visible function table.

class MTLVisibleFunctionTableDescriptor

A specification of how to create a visible function table.

protocol MTLVisibleFunctionTable

A table of shader functions visible to your app that you can pass into compute commands to customize the behavior of a shader.

class MTLIntersectionFunctionDescriptor

A description of an intersection function that performs an intersection test.

class MTLIntersectionFunctionTableDescriptor

A specification of how to create an intersection function table.

protocol MTLIntersectionFunctionTable

A table of intersection functions that Metal calls to perform ray-tracing intersection tests.

### Stitched Function Libraries

Customizing shaders using function pointers and stitching

Define custom shader behavior at runtime by creating functions from existing ones and preferentially linking to others in a dynamic library.

class MTLStitchedLibraryDescriptor

A description of a new library of procedurally generated functions.

class MTLFunctionStitchingGraph

A description of a new stitched function.

class MTLFunctionStitchingInputNode

A call graph node that describes an input to the call graph.

class MTLFunctionStitchingFunctionNode

A call graph node that describes a function call and its inputs.

protocol MTLFunctionStitchingNode

A protocol to identify call graph nodes.

class MTLFunctionStitchingAttributeAlwaysInline

An attribute to specify that Metal needs to inline all of the function calls when generating the stitched function.

protocol MTLFunctionStitchingAttribute

A protocol to identify types that customize how the Metal compiler stitches a function together.

### Compile-Time Variant Functions

class MTLFunctionConstant

A constant that specializes the behavior of a shader.

class MTLFunctionConstantValues

A set of constant values that specialize a graphics or compute function.

### Introspection Data

class MTLComputePipelineReflection

Information about the arguments of a compute function.

typealias MTLAutoreleasedComputePipelineReflection

A convenience type alias for an autoreleased compute pipeline reflection object.

class MTLRenderPipelineReflection

Information about the arguments of a graphics function.

typealias MTLAutoreleasedRenderPipelineReflection

A convenience type alias for an autoreleased pipeline reflection instance.

enum MTLBindingType

protocol MTLBinding

enum MTLBindingAccess

protocol MTLBufferBinding

protocol MTLTextureBinding

protocol MTLThreadgroupBinding

protocol MTLObjectPayloadBinding

### Function Arguments

class MTLAttribute

An object that describes an attribute defined in the stage-in argument for a shader.

class MTLVertexAttribute

An object that represents an attribute of a vertex function.

class MTLArgument

Information about an argument of a graphics or compute function.

Deprecated

typealias MTLAutoreleasedArgument

A convenience type alias for an autoreleased argument instance.

Deprecated

enum MTLArgumentType

The resource type for an argument of a function.

Deprecated

typealias MTLArgumentAccess

Function access restrictions to argument data in the shading language code.

Deprecated

### Shader Types

class MTLType

A description of a data type.

enum MTLDataType

The types of GPU functions, including shaders and compute kernels.

class MTLArrayType

A description of an array.

class MTLStructType

A description of a structure.

class MTLStructMember

An object that provides information about a field in a structure.

class MTLPointerType

A description of a pointer.

class MTLTextureReferenceType

A description of a texture.

### Shader Logging

class MTLLogStateDescriptor

An interface that represents a log state configuration.

protocol MTLLogState

A container for shader log messages.

### Errors

struct MTLLibraryError

Metal errors related to libraries.

enum Code

Error codes for Metal library errors.

let MTLLibraryErrorDomain: String

The error domain for Metal libraries.

## See Also

### Shaders

Stepping through code and inspecting variables to isolate bugs

Find the cause of your bugs by watching variables change as you step through your source code in the debugger.

Optimizing GPU performance

Find and address performance bottlenecks using the Metal debugger.

Logging shader debug messages

Print debugging messages that a shader generates using shader logging.

Using Function Specialization to Build Pipeline Variants

Create pipelines for different levels of detail from a common shader source.

