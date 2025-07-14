

- Metal
-  MTLLibraryOptimizationLevel 

Enumeration

# MTLLibraryOptimizationLevel

The optimization options for the Metal compiler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum MTLLibraryOptimizationLevel
```

## Topics

### Optimization Options

case `default`

An optimization option for the Metal compiler that prioritizes runtime performance.

case size

An optimization option for the Metal compiler that prioritizes minimizing the size of its output binaries, which may also reduce compile time.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

