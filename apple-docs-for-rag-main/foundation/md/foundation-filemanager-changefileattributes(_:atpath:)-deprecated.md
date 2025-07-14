

- Foundation
- FileManager
-  changeFileAttributes(\_:atPath:) Deprecated

Instance Method

# changeFileAttributes(\_:atPath:)

Changes the attributes of a given file or directory.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func changeFileAttributes(
    _ attributes: [AnyHashable : Any] = [:],
    atPath path: String
) -> Bool
```

Deprecated

Use setAttributes(_:ofItemAtPath:) instead.

## Parameters 

`attributes`  

A dictionary containing as keys the attributes to set for `path` and as values the corresponding value for the attribute. You can set following: `NSFileBusy`, `NSFileCreationDate`, `NSFileExtensionHidden`, `NSFileGroupOwnerAccountID`, `NSFileGroupOwnerAccountName`, `NSFileHFSCreatorCode`, `NSFileHFSTypeCode`, `NSFileImmutable`, `NSFileModificationDate`, `NSFileOwnerAccountID`, `NSFileOwnerAccountName`, `NSFilePosixPermissions`. You can change single attributes or any combination of attributes; you need not specify keys for all attributes.

For the `NSFilePosixPermissions` value, specify a file mode from the OR’d permission bit masks defined in `sys/stat.h`. See the man page for the `chmod` function (`man 2 chmod`) for an explanation.

`path`  

A path to a file or directory.

## Return Value

true if *all* changes succeed. If any change fails, returns false, but it is undefined whether any changes actually occurred.

## Discussion

As in the POSIX standard, the app either must own the file or directory or must be running as superuser for attribute changes to take effect. The method attempts to make all changes specified in attributes and ignores any rejection of an attempted modification.

The `NSFilePosixPermissions` value must be initialized with the code representing the POSIX file-permissions bit pattern. `NSFileHFSCreatorCode` and `NSFileHFSTypeCode` will only be heeded when `path` specifies a file.

### Special Considerations

Because this method does not return error information, it has been deprecated as of OS X v10.5. Use setAttributes(_:ofItemAtPath:) instead.

## See Also

### Related Documentation

func attributesOfItem(atPath: String) throws -> [FileAttributeKey : Any]

Returns the attributes of the item at a given path.

func setAttributes([FileAttributeKey : Any], ofItemAtPath: String) throws

Sets the attributes of the specified file or directory.

### Deprecated Methods

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

func replaceItemAtURL(originalItemURL: NSURL, withItemAtURL: NSURL, backupItemName: String?, options: FileManager.ItemReplacementOptions) throws -> NSURL?

Replaces the contents of the item at the specified URL in a manner that ensures no data loss occurs.

Deprecated

