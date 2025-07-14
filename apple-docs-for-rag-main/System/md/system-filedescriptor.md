

- System
-  FileDescriptor 

Structure

# FileDescriptor

An abstract handle to an input or output data resource, such as a file or a socket.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct FileDescriptor
```

## Overview

You are responsible for managing the lifetime and validity of `FileDescriptor` values, in the same way as you manage a raw C file handle.

## Topics

### Creating a File Descriptor

init(rawValue: CInt)

Creates a strongly-typed file handle from a raw C file handle.

let rawValue: CInt

The raw C file handle.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Opening a File

static func open(FilePath, FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions?, retryOnInterrupt: Bool) throws -> FileDescriptor

Opens or creates a file for reading or writing.

static func open(UnsafePointer&lt;CChar>, FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions?, retryOnInterrupt: Bool) throws -> FileDescriptor

Opens or creates a file for reading or writing.

struct AccessMode

The desired read and write access for a newly opened file.

struct OpenOptions

Options that specify behavior for a newly-opened file.

### Reading From a File

func read(into: UnsafeMutableRawBufferPointer, retryOnInterrupt: Bool) throws -> Int

Reads bytes at the current file offset into a buffer.

func read(fromAbsoluteOffset: Int64, into: UnsafeMutableRawBufferPointer, retryOnInterrupt: Bool) throws -> Int

Reads bytes at the specified offset into a buffer.

### Changing a File’s Offset

func seek(offset: Int64, from: FileDescriptor.SeekOrigin) throws -> Int64

Repositions the offset for the given file descriptor.

struct SeekOrigin

Options for specifying what a file descriptor’s offset is relative to.

### Writing To A File

func write(UnsafeRawBufferPointer, retryOnInterrupt: Bool) throws -> Int

Writes the contents of a buffer at the current file offset.

func write(toAbsoluteOffset: Int64, UnsafeRawBufferPointer, retryOnInterrupt: Bool) throws -> Int

Writes the contents of a buffer at the specified offset.

func writeAll&lt;S>(S) throws -> Int

Writes a sequence of bytes to the current offset and then updates the offset.

func writeAll&lt;S>(toAbsoluteOffset: Int64, S) throws -> Int

Writes a sequence of bytes to the given offset.

### Closing a File

func close() throws

Deletes a file descriptor.

func closeAfter&lt;R>(() throws -> R) throws -> R

Runs a closure and then closes the file descriptor, even if an error occurs.

### Encoding File Descriptors

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `Int32`.

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `Int32`.

### Comparing File Descriptors

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

var hashValue: Int

### Instance Methods

func duplicate(as: FileDescriptor?, retryOnInterrupt: Bool) throws -> FileDescriptor

Duplicates this file descriptor and return the newly created copy.

func resize(to: Int64, retryOnInterrupt: Bool) throws

Truncates or extends the file referenced by this file descriptor.

### Type Properties

static var standardError: FileDescriptor

The standard error file descriptor, with a numeric value of 2.

static var standardInput: FileDescriptor

The standard input file descriptor, with a numeric value of 0.

static var standardOutput: FileDescriptor

The standard output file descriptor, with a numeric value of 1.

### Type Methods

static func pipe() throws -> (readEnd: FileDescriptor, writeEnd: FileDescriptor)

Creates a unidirectional data channel, which can be used for interprocess communication.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Files

struct FilePath

Represents a location in the file system.

struct FilePermissions

The access permissions for a file.

