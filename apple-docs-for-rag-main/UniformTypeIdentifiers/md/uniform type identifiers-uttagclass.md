

- Uniform Type Identifiers
-  UTTagClass 

Structure

# UTTagClass

A type that represents tag classes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct UTTagClass
```

## Overview

A tag class is a label that represents the mapping of a UTType to another type system; for example, a MIME type or a file system extension.

A tag is a specific instance of a tag class. For example, the tag `txt` is an instance of the tag class UTTagClassFilenameExtension and represents the type UTTypePlainText.

UTTagClass uses an untyped `String` or CFString to refer to a tag class as a string. To get the string representation of a tag class, use its `rawValue-swift.property` property.

## Topics

### Getting a declared types mapping

static var filenameExtension: UTTagClass

A type property that returns the tag class used to map a type to a filename extension.

static var mimeType: UTTagClass

A type property that returns the tag class used to map a type to a MIME type.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Uniform type identifiers

struct UTType

A structure that represents a type of data to load, send, or receive.

class UTTypeReference

An object that represents a type of data to load, send, or receive.

