

- Metal
-  MTLIOError 

Structure

# MTLIOError

The categories of errors for creating an input/output file handle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct MTLIOError
```

## Topics

### Error Codes

static var urlInvalid: MTLIOError.Code

An error that represents a problem with a file URL.

static var `internal`: MTLIOError.Code

An error that represents a problem internal to the Metal framework.

enum Code

The error codes for creating an input/output file handle.

### Error Domain

static var errorDomain: String

The current error domain for input/output command queues.

let MTLIOErrorDomain: String

The domain for input/output command queue errors.

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

struct MTLDynamicLibraryError

Errors when compiling dynamic libraries.

struct MTLPackedFloatQuaternion

struct MTLStitchedLibraryOptions

struct NSDeviceCertification

struct NSProcessPerformanceProfile

A value describing the device’s performance profile.

