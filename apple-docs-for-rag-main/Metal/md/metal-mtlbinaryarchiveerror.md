

- Metal
-  MTLBinaryArchiveError 

Structure

# MTLBinaryArchiveError

An error that occurred when creating a binary shader archive.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct MTLBinaryArchiveError
```

## Topics

### Error Codes

static var none: MTLBinaryArchiveError.Code

An error code that represents the absence of any problems.

static var invalidFile: MTLBinaryArchiveError.Code

An error code that indicates an app is using an invalid reference to an archive file, typically related to a URL.

static var compilationFailure: MTLBinaryArchiveError.Code

An error code that indicates the archive’s inability to compile its contents, typically when serializing it to a URL.

static var unexpectedElement: MTLBinaryArchiveError.Code

An error code that indicates a problem with a configuration, typically in a descriptor or an archive’s inability to add linked functions.

static var internalError: MTLBinaryArchiveError.Code

An error code that indicates the Metal framework has an internal problem.

enum Code

Error codes when creating binary archives of compiled shader code.

### Error Domain

static var errorDomain: String

The current binary archive error domain.

let MTLBinaryArchiveDomain: String

The domain for Metal binary archive errors.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Structures

struct MTLCommandBufferError

The command buffer error codes that indicate why the GPU doesn’t finish executing a command buffer.

struct MTLComponentTransform

struct MTLCounterSampleBufferError

The error codes that indicate why a GPU driver can’t create a counter sample buffer.

struct MTLDynamicLibraryError

Errors when compiling dynamic libraries.

struct MTLIOError

The categories of errors for creating an input/output file handle.

struct MTLPackedFloatQuaternion

struct MTLStitchedLibraryOptions

struct NSDeviceCertification

struct NSProcessPerformanceProfile

A value describing the device’s performance profile.

