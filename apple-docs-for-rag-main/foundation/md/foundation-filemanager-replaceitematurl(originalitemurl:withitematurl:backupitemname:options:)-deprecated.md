

- Foundation
- FileManager
-  replaceItemAtURL(originalItemURL:withItemAtURL:backupItemName:options:) Deprecated

Instance Method

# replaceItemAtURL(originalItemURL:withItemAtURL:backupItemName:options:)

Replaces the contents of the item at the specified URL in a manner that ensures no data loss occurs.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+watchOS 2.0+visionOS 1.0+

``` source
func replaceItemAtURL(
    originalItemURL: NSURL,
    withItemAtURL newItemURL: NSURL,
    backupItemName: String? = nil,
    options: FileManager.ItemReplacementOptions = []
) throws -> NSURL?
```

Deprecated

Use replaceItemAt(_:withItemAt:backupItemName:options:) instead.

## Parameters 

`originalItemURL`  

The item containing the content you want to replace.

`newItemURL`  

The item containing the new content for `originalItemURL`. It is recommended that you put this item in a temporary directory as provided by the OS. If a temporary directory is not available, put this item in a uniquely named directory that is in the same directory as the original item.

`backupItemName`  

If provided, the name used to create a backup of the original item.

The backup is placed in the same directory as the original item. If an error occurs during the creation of the backup item, the operation fails. If there is already an item with the same name as the backup item, that item will be removed.

The backup item will be removed in the event of success unless the withoutDeletingBackupItem option is provided in options.

`options`  

The options to use during the replacement. Typically, you pass usingNewMetadataOnly for this parameter, which uses only the metadata from the new item. You can also combine the options described in FileManager.ItemReplacementOptions using the C-bitwise OR operator.

## Return Value

The URL of the new item. If no new file system object is required, the URL object in this parameter may be the same passed to the originalItemURL parameter. However, if a new file system object is required, the URL object may be different. For example, replacing an RTF document with an RTFD document requires the creation of a new file.

## Discussion

By default, the creation date, permissions, Finder label and color, and Spotlight comments of the original item are preserved on the new item. You can configure which metadata is preserved using the options parameter.

This method works only when the originalItemURL and newItemURL parameters are located on the same volume. Attempting to call this method by passing originalItemURL and newItemURL parameters that have locations on different volumes results in an error. Instead, you can call the url(for:in:appropriateFor:create:) method, passing FileManager.SearchPathDirectory.itemReplacementDirectory as the search path directory, to get a temporary URL on the destination’s volume that is suitable for use with this method.

If an error occurs and the original item is not in the original location or a temporary location, the resulting error object contains a user info dictionary with the key `"NSFileOriginalItemLocationKey"`. The value assigned to that key is an NSURL object with the location of the item. The error code is one of the file-related errors described in NSError Codes.

## See Also

### Deprecated Methods

func changeFileAttributes([AnyHashable : Any], atPath: String) -> Bool

Changes the attributes of a given file or directory.

Deprecated

func fileAttributes(atPath: String, traverseLink: Bool) -> [AnyHashable : Any]?

Returns a dictionary that describes the POSIX attributes of the file specified at a given.

Deprecated

func fileSystemAttributes(atPath: String) -> [AnyHashable : Any]?

Returns a dictionary that describes the attributes of the mounted file system on which a given path resides.

Deprecated

func directoryContents(atPath: String) -> [Any]?

Returns the directories and files (including symbolic links) contained in a given directory.

Deprecated

func createDirectory(atPath: String, attributes: [AnyHashable : Any]) -> Bool

Creates a directory (without contents) at a given path with given attributes.

Deprecated

func createSymbolicLink(atPath: String, pathContent: String) -> Bool

Creates a symbolic link identified by a given path that refers to a given location.

Deprecated

func pathContentOfSymbolicLink(atPath: String) -> String?

Returns the path of the directory or file that a symbolic link at a given path refers to.

Deprecated

func fileManager(_ fm: FileManager, shouldProceedAfterError errorInfo: [AnyHashable : Any]) -> Bool

An \`NSFileManager\` object sends this message to its handler for each error it encounters when copying, moving, removing, or linking files or directories.

Deprecated

func fileManager(_ fm: FileManager, willProcessPath path: String)

An \`NSFileManager\` object sends this message to a handler immediately before attempting to move, copy, rename, or delete, or before attempting to link to a given path.

Deprecated

