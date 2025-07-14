

- ShazamKit
- SHLibrary
-  removeItems(\_:) 

Instance Method

# removeItems(\_:)

Removes an array of media items from the user’s Shazam library.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final func removeItems(_ items: [SHMediaItem]) async throws
```

## Parameters 

`items`  

An array containing the SHMediaItem objects to remove from the library.

## Discussion

Apps can only remove media items that it added to the library with addItems(_:).

This throws SHError.Code.mediaLibrarySyncFailed if the system can’t remove at least one SHMediaItem or if an error occurred during the removal. In that case, the system doesn’t remove any items from the library.

## See Also

### Managing the items in the library

static let `default`: SHLibrary

An instance of the default Shazam library.

func addItems([SHMediaItem]) async throws

Adds an array of media items to the user’s Shazam library.

var items: [SHMediaItem]

The list of synced items in the Media Library.

