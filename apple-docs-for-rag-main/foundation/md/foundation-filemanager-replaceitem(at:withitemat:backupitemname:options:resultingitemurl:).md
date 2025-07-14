

- Foundation
- FileManager
-  replaceItem(at:withItemAt:backupItemName:options:resultingItemURL:) 

Instance Method

# replaceItem(at:withItemAt:backupItemName:options:resultingItemURL:)

Replaces the contents of the item at the specified URL in a manner that ensures no data loss occurs.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceItem(
    at originalItemURL: URL,
    withItemAt newItemURL: URL,
    backupItemName: String?,
    options: FileManager.ItemReplacementOptions = [],
    resultingItemURL resultingURL: AutoreleasingUnsafeMutablePointer?
) throws
```

## Parameters 

`originalItemURL`  

The item containing the content you want to replace.

`newItemURL`  

The item containing the new content for `originalItemURL`. It is recommended that you put this item in a temporary directory as provided by the OS. If a temporary directory is not available, put this item in a uniquely named directory that is in the same directory as the original item.

`backupItemName`  

If provided, the name used to create a backup of the original item. The backup is placed in the same directory as the original item. If an error occurs during the creation of the backup item, the operation fails. If there is already an item with the same name as the backup item, that item will be removed.

The backup item will be removed in the event of success unless the withoutDeletingBackupItem option is provided in `options`.

`options`  

The options to use during the replacement. Typically, you pass usingNewMetadataOnly for this parameter, which uses only the metadata from the new item. You can also combine the options described in FileManager.ItemReplacementOptions using the C-bitwise OR operator.

`resultingURL`  

On input, a pointer for a URL object. When the item is replaced, this pointer is set to the URL of the new item. If no new file system object is required, the URL object in this parameter may be the same passed to the `originalItemURL` parameter. However, if a new file system object is required, the URL object may be different. For example, replacing an RTF document with an RTFD document requires the creation of a new file.

## Discussion

By default, the creation date, permissions, Finder label and color, and Spotlight comments of the original item are preserved on the new item. You can configure which metadata is preserved using the `options` parameter.

This method works only when the `originalItemURL` and `newItemURL` parameters are located on the same volume. Attempting to call this method by passing `originalItemURL` and `newItemURL` parameters that have locations on different volumes results in an error. Instead, you can call the url(for:in:appropriateFor:create:) method, passing FileManager.SearchPathDirectory.itemReplacementDirectory as the search path directory, to get a temporary URL on the destination’s volume that is suitable for use with this method.

If an error occurs and the original item is not in the original location or a temporary location, the resulting error object contains a user info dictionary with the key `"NSFileOriginalItemLocationKey"`. The value assigned to that key is an NSURL object with the location of the item. The error code is one of the file-related errors described in NSError Codes.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Replacing Items

func replaceItemAt(URL, withItemAt: URL, backupItemName: String?, options: FileManager.ItemReplacementOptions) throws -> URL?

Replaces the contents of the item at the specified URL in a manner that ensures no data loss occurs.

struct ItemReplacementOptions

Options for specifying the behavior of file replacement operations.

