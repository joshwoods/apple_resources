

- Metal
-  MTLCompileOptions 

Class

# MTLCompileOptions

Compilation settings for a Metal shader library.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLCompileOptions
```

## Mentioned in 

Logging shader debug messages

Minimizing the Binary Size of a Shader Library

## Overview

You can configure the Metal compiler’s options by setting any or all of an MTLCompileOptions instance’s properties, including the following:

- Target previous OS releases by assigning the languageVersion property to an MTLLanguageVersion case.

- Set preprocessor macros for the Metal compiler by assigning a dictionary to the preprocessorMacros property.

- Choose what the Metal compiler’s optimizer prioritizes by setting the optimizationLevel property to an MTLLibraryOptimizationLevel case.

- Allow the compiler to optimize for floating-point arithmetic that may violate the IEEE 754 standard by setting mathMode to MTLMathMode.fast.

You can compile a library with your compile options instance by calling an MTLDevice instance’s makeLibrary(source:options:) or makeLibrary(source:options:completionHandler:) method.

## Topics

### Configuring the Compiler Options

var enableLogging: Bool

A Boolean value that enables shader logging.

var mathMode: MTLMathMode

An indication of whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

var mathFloatingPointFunctions: MTLMathFloatingPointFunctions

The FP32 math functions Metal uses.

var preserveInvariance: Bool

A Boolean value that indicates whether the compiler compiles vertex shaders conservatively to generate consistent position calculations.

var languageVersion: MTLLanguageVersion

The language version for interpreting the library source code.

var preprocessorMacros: [String : NSObject]?

A list of preprocessor macros to apply when compiling the library source.

var optimizationLevel: MTLLibraryOptimizationLevel

An option that tells the compiler what to prioritize when it compiles Metal shader code.

var libraries: [any MTLDynamicLibrary]?

An array of dynamic libraries the Metal compiler links against.

var fastMathEnabled: Bool

A Boolean value that indicates whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

Deprecated

### Configuring the Library Output Options

var libraryType: MTLLibraryType

The kind of library to create.

var installName: String?

For a dynamic library, the name to use when installing the library.

### Instance Properties

var allowReferencingUndefinedSymbols: Bool

var compileSymbolVisibility: MTLCompileSymbolVisibility

var maxTotalThreadsPerThreadgroup: Int

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Shader Library Management

protocol MTLLibrary

A collection of Metal shader functions.

protocol MTLDynamicLibrary

A dynamically linkable representation of compiled shader code for a specific Metal device object.

protocol MTLBinaryArchive

A container for pipeline state descriptors and their associated compiled shader code.

enum MTLLibraryType

A set of options for Metal library types.

enum MTLLanguageVersion

Metal shading language versions.

enum MTLCompileSymbolVisibility

enum MTLLibraryOptimizationLevel

The optimization options for the Metal compiler.

