

- File Provider
- NSFileProviderItemFields
-  typeAndCreator 

Type Property

# typeAndCreator

The file type and creator codes for the item.

iOS 16.0+iPadOS 16.0+macOS 12.0+visionOS 1.0+

``` source
static var typeAndCreator: NSFileProviderItemFields { get }
```

## Discussion

This property contains two values: the file type code and the creator code. The system synchronizes both codes at the same time, so define both, even if you’re just changing one.

If you modify this property, the system sets the NSFileProviderTypeAndCreator value passed to the createItem(basedOn:fields:contents:options:request:completionHandler:) or modifyItem(_:baseVersion:changedFields:contents:options:request:completionHandler:) methods. The system also writes the type and creator codes in the `FileInfo` structure, if relevant.

## See Also

### Working with Metadata

static var extendedAttributes: NSFileProviderItemFields

The item’s extended attributes.

static var fileSystemFlags: NSFileProviderItemFields

The flags describing the item’s on-disk representation.

static var tagData: NSFileProviderItemFields

The tags for the item.

static var favoriteRank: NSFileProviderItemFields

The item’s favorite rank.

