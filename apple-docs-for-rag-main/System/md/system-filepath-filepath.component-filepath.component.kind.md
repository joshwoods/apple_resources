

- System
- FilePath
- FilePath.Component
-  FilePath.Component.Kind 

Enumeration

# FilePath.Component.Kind

Whether a component is a regular file or directory name, or a special directory `.` or `..`

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum Kind
```

## Topics

### Operators

static func == (FilePath.Component.Kind, FilePath.Component.Kind) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case currentDirectory

The special directory `.`, representing the current directory.

case parentDirectory

The special directory `..`, representing the parent directory.

case regular

A file or directory name

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

