

- Foundation
- FileManager
-  createDirectory(atPath:attributes:) Deprecated

Instance Method

# createDirectory(atPath:attributes:)

Creates a directory (without contents) at a given path with given attributes.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func createDirectory(
    atPath path: String,
    attributes: [AnyHashable : Any] = [:]
) -> Bool
```

Deprecated

Use createDirectory(at:withIntermediateDirectories:attributes:) instead.

## Parameters 

`path`  

The path at which to create the new directory. The directory to be created must not yet exist, but its parent directory must exist.

`attributes`  

The file attributes for the new directory. The attributes you can set are owner and group numbers, file permissions, and modification date. If you specify `nil` for `attributes`, default values for these attributes are set (particularly write access for the creator and read access for others). For a list of keys you can include in this dictionary, Supporting Types. Some of the keys, such as `NSFileHFSCreatorCode` and `NSFileHFSTypeCode`, do not apply to directories.

## Return Value

true if the operation was successful, otherwise false.

## Discussion

Because this method does not return error information, it has been deprecated as of OS X v10.5. Use createDirectory(atPath:withIntermediateDirectories:attributes:) instead.

## See Also

### Related Documentation

func changeCurrentDirectoryPath(String) -> Bool

Changes the path of the current working directory to the specified path.

func createDirectory(atPath: String, withIntermediateDirectories: Bool, attributes: [FileAttributeKey : Any]?) throws

Creates a directory with given attributes at the specified path.

func createFile(atPath: String, contents: Data?, attributes: [FileAttributeKey : Any]?) -> Bool

Creates a file with the specified content and attributes at the given location.

func setAttributes([FileAttributeKey : Any], ofItemAtPath: String) throws

Sets the attributes of the specified file or directory.

var currentDirectoryPath: String

The path to the program’s current directory.

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

