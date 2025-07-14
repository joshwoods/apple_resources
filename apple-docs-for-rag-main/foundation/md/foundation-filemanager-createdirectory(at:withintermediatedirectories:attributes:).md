

- Foundation
- FileManager
-  createDirectory(at:withIntermediateDirectories:attributes:) 

Instance Method

# createDirectory(at:withIntermediateDirectories:attributes:)

Creates a directory with the given attributes at the specified URL.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func createDirectory(
    at url: URL,
    withIntermediateDirectories createIntermediates: Bool,
    attributes: [FileAttributeKey : Any]? = nil
) throws
```

## Parameters 

`url`  

A file URL that specifies the directory to create. If you want to specify a relative path, you must set the current working directory before creating the corresponding NSURL object. This parameter must not be `nil`.

`createIntermediates`  

If true, this method creates any nonexistent parent directories as part of creating the directory in `url`. If false, this method fails if any of the intermediate parent directories does not exist.

`attributes`  

The file attributes for the new directory. You can set the owner and group numbers, file permissions, and modification date. If you specify `nil` for this parameter, the directory is created according to the umask(2) macOS Developer Tools Manual Page of the process. The Supporting Types section lists the global constants used as keys in the `attributes` dictionary. Some of the keys, such as hfsCreatorCode and hfsTypeCode, do not apply to directories.

## Discussion

If you specify `nil` for the `attributes` parameter, this method uses a default set of values for the owner, group, and permissions of any newly created directories in the path. Similarly, if you omit a specific attribute, the default value is used. The default values for newly created directories are as follows:

- Permissions are set according to the umask of the current process. For more information, see umask.

- The owner ID is set to the effective user ID of the process.

- The group ID is set to that of the parent directory.

If you want to specify a relative path for url, you must set the current working directory before creating the corresponding NSURL object.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func setAttributes([FileAttributeKey : Any], ofItemAtPath: String) throws

Sets the attributes of the specified file or directory.

### Creating and Deleting Items

func createDirectory(atPath: String, withIntermediateDirectories: Bool, attributes: [FileAttributeKey : Any]?) throws

Creates a directory with given attributes at the specified path.

func createFile(atPath: String, contents: Data?, attributes: [FileAttributeKey : Any]?) -> Bool

Creates a file with the specified content and attributes at the given location.

func removeItem(at: URL) throws

Removes the file or directory at the specified URL.

func removeItem(atPath: String) throws

Removes the file or directory at the specified path.

func trashItem(at: URL, resultingItemURL: AutoreleasingUnsafeMutablePointer&lt;NSURL?>?) throws

Moves an item to the trash.

