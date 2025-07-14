

- Foundation
- FileManager
-  createFile(atPath:contents:attributes:) 

Instance Method

# createFile(atPath:contents:attributes:)

Creates a file with the specified content and attributes at the given location.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func createFile(
    atPath path: String,
    contents data: Data?,
    attributes attr: [FileAttributeKey : Any]? = nil
) -> Bool
```

## Parameters 

`path`  

The path for the new file.

`data`  

A data object containing the contents of the new file.

`attr`  

A dictionary containing the attributes to associate with the new file. You can use these attributes to set the owner and group numbers, file permissions, and modification date. For a list of keys, see FileAttributeKey. If you specify `nil` for `attributes`, the file is created with a set of default attributes.

## Return Value

true if the operation was successful or if the item already exists, otherwise false.

## Discussion

If you specify `nil` for the `attributes` parameter, this method uses a default set of values for the owner, group, and permissions of any newly created directories in the path. Similarly, if you omit a specific attribute, the default value is used. The default values for newly created files are as follows:

- Permissions are set according to the umask of the current process. For more information, see umask.

- The owner ID is set to the effective user ID of the process.

- The group ID is set to that of the parent directory.

If a file already exists at `path`, this method overwrites the contents of that file if the current process has the appropriate privileges to do so.

## See Also

### Related Documentation

func attributesOfItem(atPath: String) throws -> [FileAttributeKey : Any]

Returns the attributes of the item at a given path.

func contents(atPath: String) -> Data?

Returns the contents of the file at the specified path.

func setAttributes([FileAttributeKey : Any], ofItemAtPath: String) throws

Sets the attributes of the specified file or directory.

struct FileAttributeKey

Keys in dictionaries used to get and set file attributes.

### Creating and Deleting Items

func createDirectory(at: URL, withIntermediateDirectories: Bool, attributes: [FileAttributeKey : Any]?) throws

Creates a directory with the given attributes at the specified URL.

func createDirectory(atPath: String, withIntermediateDirectories: Bool, attributes: [FileAttributeKey : Any]?) throws

Creates a directory with given attributes at the specified path.

func removeItem(at: URL) throws

Removes the file or directory at the specified URL.

func removeItem(atPath: String) throws

Removes the file or directory at the specified path.

func trashItem(at: URL, resultingItemURL: AutoreleasingUnsafeMutablePointer&lt;NSURL?>?) throws

Moves an item to the trash.

