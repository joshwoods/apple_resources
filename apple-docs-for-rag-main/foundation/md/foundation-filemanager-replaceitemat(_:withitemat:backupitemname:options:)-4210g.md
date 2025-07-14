

- Foundation
- FileManager
-  replaceItemAt(\_:withItemAt:backupItemName:options:) 

Instance Method

# replaceItemAt(\_:withItemAt:backupItemName:options:)

Replaces the contents of the item at the specified URL in a manner that ensures no data loss occurs.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+Swift 4.0+

``` source
func replaceItemAt(
    _ originalItemURL: URL,
    withItemAt newItemURL: URL,
    backupItemName: String? = nil,
    options: FileManager.ItemReplacementOptions = []
) throws -> URL?
```

## Parameters 

`originalItemURL`  

The item containing the content you want to replace.

`newItemURL`  

The item containing the new content for originalItemURL. It is recommended that you put this item in a temporary directory as provided by the OS. If a temporary directory is not available, put this item in a uniquely named directory that is in the same directory as the original item.

`backupItemName`  

If provided, the name used to create a backup of the original item.

The backup is placed in the same directory as the original item. If an error occurs during the creation of the backup item, the operation fails. If there is already an item with the same name as the backup item, that item will be removed.

The backup item will be removed in the event of success unless the withoutDeletingBackupItem option is provided in options.

`options`  

The options to use during the replacement. Typically, you pass usingNewMetadataOnly for this parameter, which uses only the metadata from the new item. You can also combine the options described in FileManager.ItemReplacementOptions using the C-bitwise OR operator.

## Return Value

The URL of the new item. If no new file system object is required, the URL object in this parameter may be the same passed to the `originalItemURL` parameter. However, if a new file system object is required, the URL object may be different. For example, replacing an RTF document with an RTFD document requires the creation of a new file.

## Discussion

By default, the creation date, permissions, Finder label and color, and Spotlight comments of the original item are preserved on the new item. You can configure which metadata is preserved using the options parameter.

This method works only when the `originalItemURL` and `newItemURL` parameters are located on the same volume. Attempting to call this method by passing `originalItemURL` and `newItemURL` parameters that have locations on different volumes results in an error. Instead, you can call the url(for:in:appropriateFor:create:) method, passing FileManager.SearchPathDirectory.itemReplacementDirectory as the search path directory, to get a temporary URL on the destination’s volume that is suitable for use with this method.

If an error occurs and the original item is not in the original location or a temporary location, the resulting error object contains a user info dictionary with the key “`NSFileOriginalItemLocationKey`”. The value assigned to that key is an NSURL object with the location of the item. The error code is one of the file-related errors described in NSError Codes.

## See Also

### Replacing Items

func replaceItem(at: URL, withItemAt: URL, backupItemName: String?, options: FileManager.ItemReplacementOptions, resultingItemURL: AutoreleasingUnsafeMutablePointer&lt;NSURL?>?) throws

Replaces the contents of the item at the specified URL in a manner that ensures no data loss occurs.

struct ItemReplacementOptions

Options for specifying the behavior of file replacement operations.

