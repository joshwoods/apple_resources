

- Metal
-  MTLIOFileHandle 

Protocol

# MTLIOFileHandle

Represents a raw or compressed file, such as a resource asset file in your app’s bundle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLIOFileHandle : NSObjectProtocol
```

## Topics

### Naming a File Handle

var label: String?

An optional name for the file that the handle represents.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### I/O Command Buffers

protocol MTLIOCommandBuffer

A command buffer that contains input/output commands that work with files in the file systems and Metal resources.

typealias MTLIOCommandBufferHandler

A convenience type that defines the signature of an input/output command buffer’s completion handler.

enum MTLIOStatus

Represents the state of an input/output command buffer.

enum Code

The error codes for creating an input/output file handle.

let MTLIOErrorDomain: String

The domain for input/output command queue errors.

