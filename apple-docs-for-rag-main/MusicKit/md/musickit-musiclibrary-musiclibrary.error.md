

- MusicKit
- MusicLibrary
-  MusicLibrary.Error 

Enumeration

# MusicLibrary.Error

An error that the music library can throw upon accessing, manipulating, or requesting data from the user’s music library.

iOS 16.1+iPadOS 16.1+Mac Catalyst 17.0+macOS 14.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
enum Error
```

## Topics

### Enumeration Cases

case addToPlaylistFailed

An error that indicates a failure in the process of adding an item to a playlist.

case createPlaylistFailed

An error that indicates a failure in the process of creating a playlist.

case editPlaylistFailed

An error that indicates a failure in the process of editing a playlist.

case itemAlreadyAdded

An error indicating that the item attempting to be added to the user’s music library is already in the library.

case permissionDenied

An error that occurs when the user doesn’t consent for the current app to access their Apple Music library.

case playlistNotInLibrary

An error indicating that the playlist attempting to be added to is not in the user’s library.

case unableToAddItem

An error indicating that the item attempting to be added to the user’s music library cannot be added.

case unknown

An error indicating the ocurrence of an unknown or unexpected error.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var description: String

A textual representation of this instance.

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

