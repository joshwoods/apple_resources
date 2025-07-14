

- System
- FilePath
-  FilePath.Root 

Structure

# FilePath.Root

Represents a root of a file path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Root
```

## Overview

On Unix, a root is simply the directory separator `/`.

On Windows, a root contains the entire path prefix up to and including the final separator.

Examples:

- Unix:

  - `/`

- Windows:

  - `C:\`

  - `C:`

  - `\`

  - `\\server\share\`

  - `\\?\UNC\server\share\`

  - `\\?\Volume{12345678-abcd-1111-2222-123445789abc}\`

## Topics

### Initializers

init?(String)

Create a file path root from a string.

init?(platformString: [CInterop.PlatformChar])

Creates a file path root by copying bytes from a null-terminated platform string. It is a precondition that a null byte indicates the end of the string. The absence of a null byte will trigger a runtime error.

init?(platformString: String)Deprecated

init?(platformString: UnsafePointer&lt;CInterop.PlatformChar>)

Creates a file path root by copying bytes from a null-terminated platform string.

init?(platformString: inout CInterop.PlatformChar)Deprecated

### Instance Properties

var string: String

On Unix, this returns `"/"`.

### Instance Methods

func withPlatformString&lt;Result>((UnsafePointer&lt;CInterop.PlatformChar>) throws -> Result) rethrows -> Result

Calls the given closure with a pointer to the contents of the file path root, represented as a null-terminated platform string.

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

