

- System
- FileDescriptor
-  FileDescriptor.AccessMode 

Structure

# FileDescriptor.AccessMode

The desired read and write access for a newly opened file.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct AccessMode
```

## Topics

### Creating an Access Mode

static var readOnly: FileDescriptor.AccessMode

Opens the file for reading only.

static var readWrite: FileDescriptor.AccessMode

Opens the file for reading and writing.

static var writeOnly: FileDescriptor.AccessMode

Opens the file for writing only.

### Debugging

var description: String

A textual representation of the access mode.

var debugDescription: String

A textual representation of the access mode, suitable for debugging

### Working with C APIs

init(rawValue: CInt)

Creates a strongly-typed access mode from a raw C access mode.

var rawValue: CInt

The raw C access mode.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Comparing Access Modes

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

var hashValue: Int

### Encoding Access Modes

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

### Opening a File

static func open(FilePath, FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions?, retryOnInterrupt: Bool) throws -> FileDescriptor

Opens or creates a file for reading or writing.

static func open(UnsafePointer&lt;CChar>, FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions?, retryOnInterrupt: Bool) throws -> FileDescriptor

Opens or creates a file for reading or writing.

struct OpenOptions

Options that specify behavior for a newly-opened file.

