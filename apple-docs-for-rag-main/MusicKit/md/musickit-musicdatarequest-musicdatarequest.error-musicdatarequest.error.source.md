

- MusicKit
- MusicDataRequest
- MusicDataRequest.Error
-  MusicDataRequest.Error.Source 

Enumeration

# MusicDataRequest.Error.Source

A representation of the source of an error from Apple Music API.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Source
```

## Topics

### Operators

static func == (MusicDataRequest.Error.Source, MusicDataRequest.Error.Source) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case parameter(String)

The URI query parameter that causes the error.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

