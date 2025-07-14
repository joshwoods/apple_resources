

- Metal
-  MTLFunction 

Protocol

# MTLFunction

An object that represents a public shader function in a Metal library.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLFunction : NSObjectProtocol
```

## Overview

Use MTLFunction objects to specify which shaders a Metal pipeline calls when the GPU executes commands that specify that pipeline. For more information on creating pipeline state objects, see MTLRenderPipelineDescriptor and MTLComputePipelineDescriptor.

A MTLFunction object is a *specialized* function if the shader contains function constants, otherwise it is a *nonspecialized* function.

Don’t use standard allocation and initialization techniques to create a MTLFunction object. Instead, use the function creation methods provided by the MTLLibrary protocol. To create a nonspecialized function, call the makeFunction(name:) method.

To create a specialized function, call one of these MTLLibrary methods:

- makeFunction(name:constantValues:completionHandler:)

- makeFunction(name:constantValues:)

MTLFunction objects can use a significant amount of memory; release any strong references to them after you finish creating pipeline objects.

## Topics

### Identifying Shader Functions

var device: any MTLDevice

The device object that created the shader function.

**Required**

var label: String?

A string that identifies the shader function.

**Required**

var functionType: MTLFunctionType

The shader function’s type.

**Required**

var name: String

The function’s name.

**Required**

enum MTLFunctionType

The type of a top-level Metal Shading Language (MSL) function.

var options: MTLFunctionOptions

The options that Metal used to compile this function.

**Required**

struct MTLFunctionOptions

Options that define how Metal creates the function object.

### Identifying the Tessellation Patch

var patchType: MTLPatchType

The tessellation patch type of a post-tessellation vertex function.

**Required**

var patchControlPointCount: Int

The number of patch control points in the post-tessellation vertex function.

**Required**

enum MTLPatchType

Types of tessellation patches that can be inputs of a post-tessellation vertex function.

### Retrieving Function Attributes

var vertexAttributes: [MTLVertexAttribute]?

An array that describes the vertex input attributes to a vertex function.

**Required**

var stageInputAttributes: [MTLAttribute]?

An array that describes the input attributes to the function.

**Required**

### Retrieving Function Constants

var functionConstantsDictionary: [String : MTLFunctionConstant]

A dictionary of function constants for a specialized function.

**Required**

### Creating Argument Encoders

func makeArgumentEncoder(bufferIndex: Int) -> any MTLArgumentEncoder

Creates an argument encoder for an argument buffer that’s one of this function’s arguments.

**Required**

func makeArgumentEncoder(bufferIndex: Int, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedArgument?>?) -> any MTLArgumentEncoder

Creates an argument encoder and returns reflection information for an argument buffer that’s one of this function’s arguments

**Required**

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Shader Functions

class MTLFunctionDescriptor

A description of a function object to create.

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

