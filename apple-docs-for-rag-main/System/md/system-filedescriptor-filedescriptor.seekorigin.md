

- System
- FileDescriptor
-  FileDescriptor.SeekOrigin 

Structure

# FileDescriptor.SeekOrigin

Options for specifying what a file descriptor’s offset is relative to.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct SeekOrigin
```

## Topics

### Creating a Seek Origin

static var current: FileDescriptor.SeekOrigin

Indicates that the offset should be set to the specified number of bytes after the current location.

static var end: FileDescriptor.SeekOrigin

Indicates that the offset should be set to the size of the file plus the specified number of bytes.

static var nextHole: FileDescriptor.SeekOrigin

Indicates that the offset should be set to the next hole after the specified number of bytes.

static var nextData: FileDescriptor.SeekOrigin

Indicates that the offset should be set to the start of the next file region that isn’t a hole and is greater than or equal to the supplied offset.

static var start: FileDescriptor.SeekOrigin

Indicates that the offset should be set to the specified value.

### Debugging

var description: String

A textual representation of the seek origin.

var debugDescription: String

A textual representation of the seek origin, suitable for debugging.

### Working with C APIs

init(rawValue: CInt)

Create a strongly-typed seek origin from a raw C value.

var rawValue: CInt

The raw C value.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Comparing Seek Origins

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

var hashValue: Int

### Encoding Seek Origins

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int32`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int32`.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Changing a File’s Offset

func seek(offset: Int64, from: FileDescriptor.SeekOrigin) throws -> Int64

Repositions the offset for the given file descriptor.

