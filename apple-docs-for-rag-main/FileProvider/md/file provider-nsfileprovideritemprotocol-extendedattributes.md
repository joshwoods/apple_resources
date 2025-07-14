

- File Provider
- NSFileProviderItemProtocol
-  extendedAttributes 

Instance Property

# extendedAttributes

The extended file attributes synced by the File Provider extension.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
optional var extendedAttributes: [String : Data] { get }
```

## Discussion

The extended file attributes are part of the item’s metadata. The system sets extended attributes on dataless files, and preserves them on files that it renders dataless. The system decides which attributes to sync. To sync an attribute, it calls the `xattr_name_with_flags(_:_:)` method and passes the `XATTR_FLAG_SYNCABLE` flag. Some older attributes are also synced.

The system caps the syncable extended attributes to about 32KiB total for each item. If the extended attributes exceed this limit, the system automatically makes some of the attributes nonsyncable.

The system also decides which nonsyncable attributes it preserves on the local copy when a remote item changes. For example, it preserves attributes created by calling `xattr_name_with_flags(_:_:)` and passing `XATTR_FLAG_CONTENT_DEPENDENT` as long as the remote change didn’t modify the contentVersion property for the item’s version.

This dictionary doesn’t list extended attributes that are already covered by NSFileProviderItemFields values, like lastUsedDate or tagData. Similarly, the dictionary doesn’t include the 32 bits of Finder info stored in an extended attribute named `com.apple.FinderInfo`, because this information exists in other NSFileProviderItemProtocol properties.

Also, the resource fork is content and isn’t included in the extended attributes dictionary. If your extension detects remote changes to the resource fork, report these changes by modifying the item version’s contentVersion property.

## See Also

### Managing Metadata

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

var typeAndCreator: NSFileProviderTypeAndCreator

The file type and creator codes for the item.

