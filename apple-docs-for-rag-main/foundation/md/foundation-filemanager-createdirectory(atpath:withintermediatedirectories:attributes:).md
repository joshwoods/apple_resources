

- Foundation
- FileManager
-  createDirectory(atPath:withIntermediateDirectories:attributes:) 

Instance Method

# createDirectory(atPath:withIntermediateDirectories:attributes:)

Creates a directory with given attributes at the specified path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func createDirectory(
    atPath path: String,
    withIntermediateDirectories createIntermediates: Bool,
    attributes: [FileAttributeKey : Any]? = nil
) throws
```

## Parameters 

`path`  

A path string identifying the directory to create. You may specify a full path or a path that is relative to the current working directory. This parameter must not be `nil`.

`createIntermediates`  

If true, this method creates any nonexistent parent directories as part of creating the directory in `path`. If false, this method fails if any of the intermediate parent directories does not exist. This method also fails if any of the intermediate path elements corresponds to a file and not a directory.

`attributes`  

The file attributes for the new directory and any newly created intermediate directories. You can set the owner and group numbers, file permissions, and modification date. If you specify `nil` for this parameter or omit a particular value, one or more default values are used as described in the discussion. For a list of keys you can include in this dictionary, see Supporting Types. Some of the keys, such as hfsCreatorCode and hfsTypeCode, do not apply to directories.

## Discussion

If you specify `nil` for the `attributes` parameter, this method uses a default set of values for the owner, group, and permissions of any newly created directories in the path. Similarly, if you omit a specific attribute, the default value is used. The default values for newly created directories are as follows:

- Permissions are set according to the umask of the current process. For more information, see umask.

- The owner ID is set to the effective user ID of the process.

- The group ID is set to that of the parent directory.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func setAttributes([FileAttributeKey : Any], ofItemAtPath: String) throws

Sets the attributes of the specified file or directory.

### Creating and Deleting Items

func createDirectory(at: URL, withIntermediateDirectories: Bool, attributes: [FileAttributeKey : Any]?) throws

Creates a directory with the given attributes at the specified URL.

func createFile(atPath: String, contents: Data?, attributes: [FileAttributeKey : Any]?) -> Bool

Creates a file with the specified content and attributes at the given location.

func removeItem(at: URL) throws

Removes the file or directory at the specified URL.

func removeItem(atPath: String) throws

Removes the file or directory at the specified path.

func trashItem(at: URL, resultingItemURL: AutoreleasingUnsafeMutablePointer&lt;NSURL?>?) throws

Moves an item to the trash.

