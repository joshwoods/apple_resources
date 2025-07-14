

- Metal
- MTLCompileOptions
-  preprocessorMacros 

Instance Property

# preprocessorMacros

A list of preprocessor macros to apply when compiling the library source.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var preprocessorMacros: [String : NSObject]? { get set }
```

## Discussion

Define the macros as a dictionary where each key is a string, and the values can be either an NSString or NSNumber instance.

The default value is `nil`.

## See Also

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

var optimizationLevel: MTLLibraryOptimizationLevel

An option that tells the compiler what to prioritize when it compiles Metal shader code.

var libraries: [any MTLDynamicLibrary]?

An array of dynamic libraries the Metal compiler links against.

var fastMathEnabled: Bool

A Boolean value that indicates whether the compiler can perform optimizations for floating-point arithmetic that may violate the IEEE 754 standard.

Deprecated

