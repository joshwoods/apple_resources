

- System
-  FilePath 

Structure

# FilePath

Represents a location in the file system.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct FilePath
```

## Overview

This structure recognizes directory separators (e.g. `/`), roots, and requires that the content terminates in a NUL (`0x0`). Beyond that, it does not give any meaning to the bytes that it contains. The file system defines how the content is interpreted; for example, by its choice of string encoding.

On construction, `FilePath` will normalize separators by removing redundant intermediary separators and stripping any trailing separators. On Windows, `FilePath` will also normalize forward slashes `/` into backslashes `\`, as preferred by the platform.

The code below creates a file path from a string literal, and then uses it to open and append to a log file:

```
let message: String = "This is a log message."
let path: FilePath = "/tmp/log"
let fd = try FileDescriptor.open(path, .writeOnly, options: .append)
try fd.closeAfter { try fd.writeAll(message.utf8) }
```

File paths conform to the Equatable and Hashable protocols by performing the protocols’ operations on their raw byte contents. This conformance allows file paths to be used, for example, as keys in a dictionary. However, the rules for path equivalence are file-system–specific and have additional considerations like case insensitivity, Unicode normalization, and symbolic links.

## Topics

### Creating a File Path

init()

Creates an empty, null-terminated path.

init(stringLiteral: String)

Creates a file path from a string literal.

init(extendedGraphemeClusterLiteral: Self.StringLiteralType)

init(unicodeScalarLiteral: Self.ExtendedGraphemeClusterLiteralType)

### Working with File Paths

var length: Int

The length of the file path, excluding the null terminator.

var description: String

A textual representation of the file path.

var debugDescription: String

A textual representation of the file path, suitable for debugging.

### Interacting with C APIs

func withCString&lt;Result>((UnsafePointer&lt;CChar>) throws -> Result) rethrows -> Result

For backwards compatibility only. This function is equivalent to the preferred `withPlatformString`.

### Comparing File Paths

static func == (FilePath, FilePath) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Encoding File Paths

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Structures

struct Component

Represents an individual, non-root component of a file path.

struct ComponentView

A bidirectional, range replaceable collection of the non-root components that make up a file path.

struct Root

Represents a root of a file path.

### Initializers

init?(URL)

Creates a file path from a URL

init(String)

Creates a file path from a string.

init(cString: [CChar])Deprecated

init(cString: String)Deprecated

init(cString: UnsafePointer&lt;CChar>)

For backwards compatibility only. This initializer is equivalent to the preferred `FilePath(platformString:)`.

Deprecated

init(cString: inout CChar)Deprecated

init(platformString: inout CInterop.PlatformChar)Deprecated

init(platformString: UnsafePointer&lt;CInterop.PlatformChar>)

Creates a file path by copying bytes from a null-terminated platform string.

init(platformString: String)Deprecated

init(platformString: [CInterop.PlatformChar])

Creates a file path by copying bytes from a null-terminated platform string.

init&lt;C>(root: FilePath.Root?, C)

Create a file path from a root and a collection of components.

init(root: FilePath.Root?, FilePath.ComponentView.SubSequence)

Create a file path from an optional root and a slice of another path’s components.

init(root: FilePath.Root?, components: FilePath.Component...)

Create a file path from a root and any number of components.

### Instance Properties

var components: FilePath.ComponentView

View the non-root components that make up this path.

var `extension`: String?

The extension of the file or directory last component.

var isAbsolute: Bool

Returns true if this path uniquely identifies the location of a file without reference to an additional starting location.

var isEmpty: Bool

Whether this path is empty

var isLexicallyNormal: Bool

Whether the path is in lexical-normal form, that is `.` and `..` components have been collapsed lexically (i.e. without following symlinks).

var isRelative: Bool

Returns true if this path is not absolute (see `isAbsolute`).

var lastComponent: FilePath.Component?

Returns the final component of the path. Returns `nil` if the path is empty or only contains a root.

var root: FilePath.Root?

Returns the root of a path if there is one, otherwise `nil`.

var stem: String?

The non-extension portion of the file or directory last component.

var string: String

Creates a string by interpreting the path’s content as UTF-8 on Unix and UTF-16 on Windows.

### Instance Methods

func append&lt;C>(C)

Append `components` on to the end of this path.

func append(String)

Append the contents of `other`, ignoring any spurious leading separators.

func append(FilePath.Component)

Append a `component` on to the end of this path.

func appending(String) -> FilePath

Non-mutating version of `append(_:String)`.

func appending(FilePath.Component) -> FilePath

Non-mutating version of `append(_:Component)`.

func appending&lt;C>(C) -> FilePath

Non-mutating version of `append(_:C)`.

func ends(with: FilePath) -> Bool

Returns whether `other` is a suffix of `self`, only considering whole path components.

func lexicallyNormalize()

Collapse `.` and `..` components lexically (i.e. without following symlinks).

func lexicallyNormalized() -> FilePath

Returns a copy of `self` in lexical-normal form, that is `.` and `..` components have been collapsed lexically (i.e. without following symlinks). See `lexicallyNormalize`

func lexicallyResolving(FilePath) -> FilePath?

Create a new `FilePath` by resolving `subpath` relative to `self`, ensuring that the result is lexically contained within `self`.

func push(FilePath)

If `other` does not have a root, append each component of `other`. If `other` has a root, replaces `self` with other.

func pushing(FilePath) -> FilePath

Non-mutating version of `push()`.

func removeAll(keepingCapacity: Bool)

Remove the contents of the path, keeping the null terminator.

func removeLastComponent() -> Bool

In-place mutating variant of `removingLastComponent`.

func removePrefix(FilePath) -> Bool

If `prefix` is a prefix of `self`, removes it and returns `true`. Otherwise returns `false`.

func removingLastComponent() -> FilePath

Creates a new path with everything up to but not including `lastComponent`.

func removingRoot() -> FilePath

Creates a new path containing just the components, i.e. everything after `root`.

func reserveCapacity(Int)

Reserve enough storage space to store `minimumCapacity` platform characters.

func starts(with: FilePath) -> Bool

Returns whether `other` is a prefix of `self`, only considering whole path components.

func withPlatformString&lt;Result>((UnsafePointer&lt;CInterop.PlatformChar>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the file path, represented as a null-terminated platform string.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

ExpressibleByUnicodeScalarLiteral Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- Sendable

## See Also

### Files

struct FileDescriptor

An abstract handle to an input or output data resource, such as a file or a socket.

struct FilePermissions

The access permissions for a file.

