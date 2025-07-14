

- Metal
-  MTLLanguageVersion 

Enumeration

# MTLLanguageVersion

Metal shading language versions.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MTLLanguageVersion
```

## Topics

### Version Numbers

case version1_1

Version 1.1 of the Metal shading language.

case version1_2

Version 1.2 of the Metal shading language.

case version2_0

Version 2.0 of the Metal shading language.

case version2_1

Version 2.1 of the Metal shading language.

case version2_2

Version 2.2 of the Metal shading language.

case version2_3

Version 2.3 of the Metal shading language.

case version2_4

Version 2.4 of the Metal shading language.

case version3_0

Version 3.0 of the Metal shading language.

case version3_1

Version 3.1 of the Metal shading language.

case version3_2

Version 3.2 of the Metal shading language.

case version1_0

Version 1.0 of the Metal shading language.

Deprecated

### Initializers

init?(rawValue: UInt)

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

enum MTLCompileSymbolVisibility

enum MTLLibraryOptimizationLevel

The optimization options for the Metal compiler.

