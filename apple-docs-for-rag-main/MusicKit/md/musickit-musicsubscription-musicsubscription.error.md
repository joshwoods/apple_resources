

- MusicKit
- MusicSubscription
-  MusicSubscription.Error 

Enumeration

# MusicSubscription.Error

An error that MusicKit can throw upon requesting the current music subscription of the user.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Error
```

## Topics

### Enumeration Cases

case permissionDenied

An error indicating that the user doesn’t consent for your app to access their Apple Music data.

case privacyAcknowledgementRequired

An error indicating that the user needs to acknowledge the most-recent privacy policy for Apple Music.

case unknown

An error indicating the ocurrence of an unknown or unexpected error.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var errorDescription: String?

A localized message describing what error occurred.

var failureReason: String?

A localized message describing the reason for the failure.

var helpAnchor: String?

A localized message providing “help” text if the user requests help.

var rawValue: String

The corresponding value of the raw type.

var recoverySuggestion: String?

A localized message describing how one might recover from the failure.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

Error Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Error
- Hashable
- LocalizedError
- RawRepresentable
- Sendable

