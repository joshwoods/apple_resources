

- Metal
-  MTLLibraryType 

Enumeration

# MTLLibraryType

A set of options for Metal library types.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MTLLibraryType
```

## Topics

### Library Options

case executable

A library that can create pipeline state objects.

case dynamic

A library that you can dynamically link to from other libraries.

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

enum MTLLanguageVersion

Metal shading language versions.

enum MTLCompileSymbolVisibility

enum MTLLibraryOptimizationLevel

The optimization options for the Metal compiler.

