

- Foundation
- FileManager
-  directoryContents(atPath:) Deprecated

Instance Method

# directoryContents(atPath:)

Returns the directories and files (including symbolic links) contained in a given directory.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func directoryContents(atPath path: String) -> [Any]?
```

Deprecated

Use contentsOfDirectory(atPath:) instead.

## Parameters 

`path`  

A path to a directory.

## Return Value

An array of NSString objects identifying the directories and files (including symbolic links) contained in `path`. Returns an empty array if the directory exists but has no contents. Returns `nil` if the directory specified at `path` does not exist or there is some other error accessing it.

## Discussion

The search is shallow, and therefore does not return the contents of any subdirectories and does not traverse symbolic links in the specified directory. This returned array does not contain strings for the current directory (”`.`”), parent directory (”`..`”), or resource forks (begin with “.\_”).

### Special Considerations

Because this method does not return error information, it has been deprecated as of OS X v10.5. Use contentsOfDirectory(atPath:) instead.

## See Also

### Related Documentation

var currentDirectoryPath: String

The path to the program’s current directory.

func fileExists(atPath: String, isDirectory: UnsafeMutablePointer&lt;ObjCBool>?) -> Bool

Returns a Boolean value that indicates whether a file or directory exists at a specified path.

func subpaths(atPath: String) -> [String]?

Returns an array of strings identifying the paths for all items in the specified directory.

func contentsOfDirectory(atPath: String) throws -> [String]

Performs a shallow search of the specified directory and returns the paths of any contained items.

func enumerator(atPath: String) -> FileManager.DirectoryEnumerator?

Returns a directory enumerator object that can be used to perform a deep enumeration of the directory at the specified path.

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

