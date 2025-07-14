

- Metal
- MTLDynamicLibraryError
-  invalidFile 

Type Property

# invalidFile

An error code that indicates an app is using an invalid reference to a library file, typically related to a URL.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
static var invalidFile: MTLDynamicLibraryError.Code { get }
```

## See Also

### Error Codes

static var none: MTLDynamicLibraryError.Code

An error code that represents the absence of any problems.

static var compilationFailure: MTLDynamicLibraryError.Code

An error code that indicates Metal couldn’t compile a dynamic library.

static var unresolvedInstallName: MTLDynamicLibraryError.Code

An error code that indicates Metal couldn’t resolve the installation name for a new dynamic library.

static var dependencyLoadFailure: MTLDynamicLibraryError.Code

An error code that indicates a dynamic library couldn’t link to other dynamic libraries.

static var unsupported: MTLDynamicLibraryError.Code

An error code that indicates the GPU device doesn’t support dynamic libraries.

enum Code

Error codes that Metal can generate when creating dynamic libraries.

