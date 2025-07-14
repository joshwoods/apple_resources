

- Foundation
- FileManager
-  createSymbolicLink(atPath:pathContent:) Deprecated

Instance Method

# createSymbolicLink(atPath:pathContent:)

Creates a symbolic link identified by a given path that refers to a given location.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func createSymbolicLink(
    atPath path: String,
    pathContent otherpath: String
) -> Bool
```

Deprecated

Use createSymbolicLink(at:withDestinationURL:) instead.

## Parameters 

`path`  

The path for a symbolic link.

`otherpath`  

The path to which `path` should refer.

## Return Value

true if the operation is successful, otherwise false. Returns false if a file, directory, or symbolic link identical to `path` already exists.

## Discussion

Creates a symbolic link identified by `path` that refers to the location `otherPath` in the file system.

### Special Considerations

Because this method does not return error information, it has been deprecated as of OS X v10.5. Use createSymbolicLink(atPath:withDestinationPath:) instead.

## See Also

### Related Documentation

func removeItem(atPath: String) throws

Removes the file or directory at the specified path.

func destinationOfSymbolicLink(atPath: String) throws -> String

Returns the path of the item pointed to by a symbolic link.

func createSymbolicLink(atPath: String, withDestinationPath: String) throws

Creates a symbolic link that points to the specified destination.

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

