

- Metal
- MTLIOError
-  MTLIOError.Code 

Enumeration

# MTLIOError.Code

The error codes for creating an input/output file handle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error Codes

case urlInvalid

An error code that represents a problem with a file URL.

case `internal`

An error code that represents a problem internal to the Metal framework.

case urlInvalid

An error code that represents a problem with a file URL.

case `internal`

An error code that represents a problem internal to the Metal framework.

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

### I/O Command Buffers

protocol MTLIOCommandBuffer

A command buffer that contains input/output commands that work with files in the file systems and Metal resources.

protocol MTLIOFileHandle

Represents a raw or compressed file, such as a resource asset file in your app’s bundle.

typealias MTLIOCommandBufferHandler

A convenience type that defines the signature of an input/output command buffer’s completion handler.

enum MTLIOStatus

Represents the state of an input/output command buffer.

let MTLIOErrorDomain: String

The domain for input/output command queue errors.

