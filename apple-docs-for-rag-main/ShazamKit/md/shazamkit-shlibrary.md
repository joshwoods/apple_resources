

- ShazamKit
-  SHLibrary 

Class

# SHLibrary

An object that represents a user’s synced Shazam library.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final class SHLibrary
```

## Topics

### Managing the items in the library

static let `default`: SHLibrary

An instance of the default Shazam library.

func addItems([SHMediaItem]) async throws

Adds an array of media items to the user’s Shazam library.

func removeItems([SHMediaItem]) async throws

Removes an array of media items from the user’s Shazam library.

var items: [SHMediaItem]

The list of synced items in the Media Library.

## Relationships

### Conforms To

- Copyable
- Observable
- Sendable

## See Also

### Update the user’s Shazam library

class SHMediaLibrary

An object that represents the user’s Shazam library.

Deprecated

