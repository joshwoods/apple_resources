

- ShazamKit
- SHLibrary
-  items 

Instance Property

# items

The list of synced items in the Media Library.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor
final var items: [SHMediaItem] { get }
```

## See Also

### Managing the items in the library

static let `default`: SHLibrary

An instance of the default Shazam library.

func addItems([SHMediaItem]) async throws

Adds an array of media items to the user’s Shazam library.

func removeItems([SHMediaItem]) async throws

Removes an array of media items from the user’s Shazam library.

