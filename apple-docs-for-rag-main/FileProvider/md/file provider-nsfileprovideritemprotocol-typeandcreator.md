

- File Provider
- NSFileProviderItemProtocol
-  typeAndCreator 

Instance Property

# typeAndCreator

The file type and creator codes for the item.

iOS 16.0+iPadOS 16.0+macOS 12.0+visionOS 1.0+

``` source
optional var typeAndCreator: NSFileProviderTypeAndCreator { get }
```

## Discussion

This property contains two values: the file type code and the creator code. The system synchronizes both codes at the same time, so define both, even if you’re just changing one.

If you modify this property, the system sets the NSFileProviderTypeAndCreator value passed to the createItem(basedOn:fields:contents:options:request:completionHandler:) or modifyItem(_:baseVersion:changedFields:contents:options:request:completionHandler:) methods. The system also writes the type and creator codes in the `FileInfo` structure, if relevant.

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

var favoriteRank: NSNumber?

A 64-bit, unsigned integer indicating the order of the favorite item in the Favorites list.

let NSFileProviderFavoriteRankUnranked: UInt64

A value that indicates that the item is not ranked.

