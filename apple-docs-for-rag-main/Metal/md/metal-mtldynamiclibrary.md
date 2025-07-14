

- Metal
-  MTLDynamicLibrary 

Protocol

# MTLDynamicLibrary

A dynamically linkable representation of compiled shader code for a specific Metal device object.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
protocol MTLDynamicLibrary : NSObjectProtocol
```

## Topics

### Identifying the Library

var device: any MTLDevice

The Metal device object that created the dynamic library.

**Required**

var installName: String

A file path for this dynamic library.

**Required**

var label: String?

A string that identifies the library.

**Required**

### Saving a Dynamic Library to a File

func serialize(to: URL) throws

Writes the contents of the dynamic library to a file.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Shader Library Management

protocol MTLLibrary

A collection of Metal shader functions.

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

