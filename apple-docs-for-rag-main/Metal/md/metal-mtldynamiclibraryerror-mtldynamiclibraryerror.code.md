

- Metal
- MTLDynamicLibraryError
-  MTLDynamicLibraryError.Code 

Enumeration

# MTLDynamicLibraryError.Code

Error codes that Metal can generate when creating dynamic libraries.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error Codes

case none

An error code that represents the absence of any problems.

case invalidFile

An error code that indicates an app is using an invalid reference to a library file, typically related to a URL.

case compilationFailure

An error code that indicates Metal couldn’t compile a dynamic library.

case unresolvedInstallName

An error code that indicates Metal couldn’t resolve the installation name for a new dynamic library.

case dependencyLoadFailure

An error code that indicates a dynamic library couldn’t link to other dynamic libraries.

case unsupported

An error code that indicates the GPU device doesn’t support dynamic libraries.

case none

An error code that represents the absence of any problems.

case invalidFile

An error code that indicates an app is using an invalid reference to a library file, typically related to a URL.

case compilationFailure

An error code that indicates Metal couldn’t compile a dynamic library.

case unresolvedInstallName

An error code that indicates Metal couldn’t resolve the installation name for a new dynamic library.

case dependencyLoadFailure

An error code that indicates a dynamic library couldn’t link to other dynamic libraries.

case unsupported

An error code that indicates the GPU device doesn’t support dynamic libraries.

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

### Error Codes

static var none: MTLDynamicLibraryError.Code

An error code that represents the absence of any problems.

static var invalidFile: MTLDynamicLibraryError.Code

An error code that indicates an app is using an invalid reference to a library file, typically related to a URL.

static var compilationFailure: MTLDynamicLibraryError.Code

An error code that indicates Metal couldn’t compile a dynamic library.

static var unresolvedInstallName: MTLDynamicLibraryError.Code

An error code that indicates Metal couldn’t resolve the installation name for a new dynamic library.

static var dependencyLoadFailure: MTLDynamicLibraryError.Code

An error code that indicates a dynamic library couldn’t link to other dynamic libraries.

static var unsupported: MTLDynamicLibraryError.Code

An error code that indicates the GPU device doesn’t support dynamic libraries.

