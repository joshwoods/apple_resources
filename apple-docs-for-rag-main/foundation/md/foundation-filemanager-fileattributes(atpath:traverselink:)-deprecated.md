

- Foundation
- FileManager
-  fileAttributes(atPath:traverseLink:) Deprecated

Instance Method

# fileAttributes(atPath:traverseLink:)

Returns a dictionary that describes the POSIX attributes of the file specified at a given.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func fileAttributes(
    atPath path: String,
    traverseLink yorn: Bool
) -> [AnyHashable : Any]?
```

Deprecated

Use attributesOfItem(atPath:) instead.

## Parameters 

`path`  

A file path.

`yorn`  

If `path` is not a symbolic link, this parameter has no effect. If `path` is a symbolic link, then:

- If true the attributes of the linked-to file are returned, or if the link points to a nonexistent file the method returns `nil`.

- If false, the attributes of the symbolic link are returned.

## Return Value

An `NSDictionary` object that describes the POSIX attributes of the file specified at `path`. The keys in the dictionary are described in `File Attribute Keys`. If there is no item at `path`, returns `nil`.

## Discussion

This code example gets several attributes of a file and logs them.

```
NSFileManager *fileManager = [[NSFileManager alloc] init];
NSString *path = @"/tmp/List";
NSDictionary *fileAttributes = [fileManager fileAttributesAtPath:path traverseLink:YES];

if (fileAttributes != nil) {
    NSNumber *fileSize;
    NSString *fileOwner;
    NSDate *fileModDate;
    if (fileSize = [fileAttributes objectForKey:NSFileSize]) {
        NSLog(@"File size: %qi\n", [fileSize unsignedLongLongValue]);
    }
    if (fileOwner = [fileAttributes objectForKey:NSFileOwnerAccountName]) {
        NSLog(@"Owner: %@\n", fileOwner);
    }
    if (fileModDate = [fileAttributes objectForKey:NSFileModificationDate]) {
        NSLog(@"Modification date: %@\n", fileModDate);
    }
}
else {
    NSLog(@"Path (%@) is invalid.", path);
}
```

As a convenience, `NSDictionary` provides a set of methods (declared as a category in `NSFileManager.h`) for quickly and efficiently obtaining attribute information from the returned dictionary: fileGroupOwnerAccountName(), fileModificationDate(), fileOwnerAccountName(), filePosixPermissions(), fileSize(), fileSystemFileNumber(), fileSystemNumber(), and fileType(). For example, you could rewrite the file modification statement in the code example above as:

```
if (fileModDate = [fileAttributes fileModificationDate])
    NSLog(@"Modification date: %@\n", fileModDate);
```

### Special Considerations

Because this method does not return error information, it has been deprecated as of OS X v10.5. Use attributesOfItem(atPath:) instead.

## See Also

### Related Documentation

func attributesOfItem(atPath: String) throws -> [FileAttributeKey : Any]

Returns the attributes of the item at a given path.

func setAttributes([FileAttributeKey : Any], ofItemAtPath: String) throws

Sets the attributes of the specified file or directory.

### Deprecated Methods

func changeFileAttributes([AnyHashable : Any], atPath: String) -> Bool

Changes the attributes of a given file or directory.

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

