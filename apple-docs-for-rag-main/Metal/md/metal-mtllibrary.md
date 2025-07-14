

- Metal
-  MTLLibrary 

Protocol

# MTLLibrary

A collection of Metal shader functions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLLibrary : NSObjectProtocol
```

## Mentioned in 

Building a Shader Library by Precompiling Source Files

Logging shader debug messages

## Overview

A MTLLibrary object contains Metal shading language source code compiled during an app’s build process or at runtime from a text string.

Don’t implement this protocol yourself; instead, use the library creation methods provided by the MTLDevice protocol. To create a MTLLibrary from a precompiled Metal library binary, call one of these MTLDevice methods:

- makeDefaultLibrary()

- makeLibrary(filepath:)

- makeLibrary(data:)

To create a MTLLibrary by compiling source code at runtime, call one of these MTLDevice methods:

- makeLibrary(source:options:completionHandler:)

- makeLibrary(source:options:)

## Topics

### Querying Basic Library Attributes

var installName: String?

The installation name for a dynamic library.

**Required**

var type: MTLLibraryType

The library’s basic type.

**Required**

### Querying Library Contents

var functionNames: [String]

The names of all public functions in the library.

**Required**

### Creating Shader Function Objects

func makeFunction(name: String) -> (any MTLFunction)?

Creates an object that represents a shader function in the library.

**Required**

func makeFunction(name: String, constantValues: MTLFunctionConstantValues, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates a specialized shader function.

**Required**

func makeFunction(name: String, constantValues: MTLFunctionConstantValues) throws -> any MTLFunction

Synchronously creates a specialized shader function.

**Required**

func makeFunction(descriptor: MTLFunctionDescriptor, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates an object representing a shader function, using the specified descriptor.

**Required**

func makeFunction(descriptor: MTLFunctionDescriptor) throws -> any MTLFunction

Synchronously creates an object representing a shader function, using the specified descriptor.

**Required**

### Creating Intersection Function Objects

func makeIntersectionFunction(descriptor: MTLIntersectionFunctionDescriptor, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates an object representing a ray-tracing intersection function, using the specified descriptor.

**Required**

func makeIntersectionFunction(descriptor: MTLIntersectionFunctionDescriptor) throws -> any MTLFunction

Synchronously creates an object representing a ray-tracing intersection function, using the specified descriptor.

**Required**

### Identifying the Library

var device: any MTLDevice

The Metal device object that created the library.

**Required**

var label: String?

A string that identifies the library.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Shader Library Management

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

