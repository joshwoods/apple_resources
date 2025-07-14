

- System
- FilePath
-  FilePath.Component 

Structure

# FilePath.Component

Represents an individual, non-root component of a file path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Component
```

## Overview

Components can be one of the special directory components (`.` or `..`) or a file or directory name. Components are never empty and never contain the directory separator.

Example:

```
var path: FilePath = "/tmp"
let file: FilePath.Component = "foo.txt"
file.kind == .regular           // true
file.extension                  // "txt"
path.append(file)               // path is "/tmp/foo.txt"
```

## Topics

### Initializers

init?(String)

Create a file path component from a string.

init?(platformString: [CInterop.PlatformChar])

Creates a file path component by copying bytes from a null-terminated platform string. It is a precondition that a null byte indicates the end of the string. The absence of a null byte will trigger a runtime error.

init?(platformString: inout CInterop.PlatformChar)Deprecated

init?(platformString: String)Deprecated

init?(platformString: UnsafePointer&lt;CInterop.PlatformChar>)

Creates a file path component by copying bytes from a null-terminated platform string.

### Instance Properties

var `extension`: String?

The extension of this file or directory component.

var kind: FilePath.Component.Kind

The kind of this component

var stem: String

The non-extension portion of this file or directory component.

var string: String

Creates a string by interpreting the component’s content as UTF-8 on Unix and UTF-16 on Windows.

### Instance Methods

func withPlatformString&lt;Result>((UnsafePointer&lt;CInterop.PlatformChar>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the file path component, represented as a null-terminated platform string.

### Enumerations

enum Kind

Whether a component is a regular file or directory name, or a special directory `.` or `..`

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

