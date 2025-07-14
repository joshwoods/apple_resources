

- Metal
-  MTLDynamicLibraryError 

Structure

# MTLDynamicLibraryError

Errors when compiling dynamic libraries.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct MTLDynamicLibraryError
```

## Topics

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

enum Code

Error codes that Metal can generate when creating dynamic libraries.

### Error Domain

static var errorDomain: String

The current dynamic library error domain.

let MTLDynamicLibraryDomain: String

The domain for Metal dynamic library errors.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Structures

struct MTLBinaryArchiveError

An error that occurred when creating a binary shader archive.

struct MTLCommandBufferError

The command buffer error codes that indicate why the GPU doesn’t finish executing a command buffer.

struct MTLComponentTransform

struct MTLCounterSampleBufferError

The error codes that indicate why a GPU driver can’t create a counter sample buffer.

struct MTLIOError

The categories of errors for creating an input/output file handle.

struct MTLPackedFloatQuaternion

struct MTLStitchedLibraryOptions

struct NSDeviceCertification

struct NSProcessPerformanceProfile

A value describing the device’s performance profile.

