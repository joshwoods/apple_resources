

- File Provider
- NSFileProviderItemProtocol
-  userInfo 

Instance Property

# userInfo

A property list that contains additional data about the item.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
optional var userInfo: [AnyHashable : Any]? { get }
```

## Discussion

The `userInfo` data is often used by the predicate for actions defined by the File Provider UI extension. For more information, see `Adding Actions to the Context Menu`.

The `userInfo` dictionary can only accept entries with numbers (including Boolean values), dates, or strings as either the key or the value.

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

var favoriteRank: NSNumber?

A 64-bit, unsigned integer indicating the order of the favorite item in the Favorites list.

let NSFileProviderFavoriteRankUnranked: UInt64

A value that indicates that the item is not ranked.

var typeAndCreator: NSFileProviderTypeAndCreator

The file type and creator codes for the item.

