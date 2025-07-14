

- MusicKit
- MusicDataRequest
-  MusicDataRequest.Error 

Structure

# MusicDataRequest.Error

An error that the Apple Music API returns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Error
```

## Topics

### Instance Properties

let code: Int

The specific code for the underlying cause of the error.

let detailText: String

Additional detailed information about the cause of the error.

let id: String

The identifier for the error.

let originalResponse: MusicDataResponse

The original response that contains the error.

let source: MusicDataRequest.Error.Source?

The source of the error.

let status: Int

The HTTP status code for the error.

let title: String

A developer-friendly title for the error.

### Enumerations

enum Source

A representation of the source of an error from Apple Music API.

### Default Implementations

CustomStringConvertible Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Error
- Sendable

