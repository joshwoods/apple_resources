

- File Provider
- NSFileProviderItemProtocol
-  favoriteRank 

Instance Property

# favoriteRank

A 64-bit, unsigned integer indicating the order of the favorite item in the Favorites list.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
@NSCopying
optional var favoriteRank: NSNumber? { get }
```

## See Also

### Managing Metadata

var extendedAttributes: [String : Data]

The extended file attributes synced by the File Provider extension.

var fileSystemFlags: NSFileProviderFileSystemFlags

Flags that define an item’s on-disk properties and its appearance in the user interface.

struct NSFileProviderFileSystemFlags

Flags that define an item’s on-disk properties and its appearance in the user interface.

var tagData: Data?

An abstract data blob representing the tags associated with the item.

var userInfo: [AnyHashable : Any]?

A property list that contains additional data about the item.

let NSFileProviderFavoriteRankUnranked: UInt64

A value that indicates that the item is not ranked.

var typeAndCreator: NSFileProviderTypeAndCreator

The file type and creator codes for the item.

