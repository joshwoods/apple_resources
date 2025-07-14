

- Metal
- MTLCompileOptions
-  fastMathEnabled Deprecated

Instance Property

# fastMathEnabled

A Boolean value that indicates whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0Deprecated

``` source
var fastMathEnabled: Bool { get set }
```

Deprecated

Use mathMode instead.

## Discussion

The default value is true. A true value also enables the high-precision variant of math functions for single-precision floating-point scalar and vector types.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

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

