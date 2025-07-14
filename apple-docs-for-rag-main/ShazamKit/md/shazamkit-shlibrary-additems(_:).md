

- ShazamKit
- SHLibrary
-  addItems(\_:) 

Instance Method

# addItems(\_:)

Adds an array of media items to the user’s Shazam library.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final func addItems(_ items: [SHMediaItem]) async throws
```

## Parameters 

`items`  

An array containing the SHMediaItem objects to add to the library.

## Discussion

The library only accepts media items with a shazamID. The `shazamID` must be a numeric only string.

This throws SHError.Code.mediaLibrarySyncFailed if the system can’t add at least one SHMediaItem or if an error occurred during the addition. In that case, the system doesn’t add any items to the library.

## See Also

### Managing the items in the library

static let `default`: SHLibrary

An instance of the default Shazam library.

func removeItems([SHMediaItem]) async throws

Removes an array of media items from the user’s Shazam library.

var items: [SHMediaItem]

The list of synced items in the Media Library.

