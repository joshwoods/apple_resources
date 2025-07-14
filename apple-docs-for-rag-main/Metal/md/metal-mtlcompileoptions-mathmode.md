

- Metal
- MTLCompileOptions
-  mathMode 

Instance Property

# mathMode

An indication of whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var mathMode: MTLMathMode { get set }
```

## Discussion

This property replaces the fastMathEnabled property.

If fastMathEnabled is `true`, the system sets mathMode to MTLMathMode.fast and mathFloatingPointFunctions to MTLMathFloatingPointFunctions.fast.

If fastMathEnabled is `false`, the system sets mathMode to MTLMathMode.safe and mathFloatingPointFunctions to MTLMathFloatingPointFunctions.precise.

Subsequent calls to mathMode or mathFloatingPointFunctions set the variables directly.

## Topics

### Supporting Types

enum MTLMathMode

An indication of whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

## See Also

### Configuring the Compiler Options

var enableLogging: Bool

A Boolean value that enables shader logging.

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

