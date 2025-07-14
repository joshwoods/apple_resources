

- Metal
-  MTLIOStatus 

Enumeration

# MTLIOStatus

Represents the state of an input/output command buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum MTLIOStatus
```

## Topics

### I/O Command Queue States

case pending

Indicates the GPU hasn’t finished executing the input/output command buffer.

case complete

Indicates the GPU has successfully finished executing the input/output command buffer.

case cancelled

Indicates the GPU has successfully abandoned the input/output command buffer.

case error

Indicates the GPU experienced a problem with the input/output command buffer.

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

enum Code

The error codes for creating an input/output file handle.

let MTLIOErrorDomain: String

The domain for input/output command queue errors.

