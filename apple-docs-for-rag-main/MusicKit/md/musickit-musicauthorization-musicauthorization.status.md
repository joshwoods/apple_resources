

- MusicKit
- MusicAuthorization
-  MusicAuthorization.Status 

Enumeration

# MusicAuthorization.Status

A value that indicates the authorization status the user sets for the current app to access their Apple Music data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Status
```

## Topics

### Enumeration Cases

case authorized

The user granted permission for the current app to use MusicKit.

case denied

The user denied permission for the current app to use MusicKit.

case notDetermined

The user has yet to decide whether to authorize the current app to use MusicKit.

case restricted

Apps on this device can’t access MusicKit in a way that the user can’t change.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable
- Sendable

