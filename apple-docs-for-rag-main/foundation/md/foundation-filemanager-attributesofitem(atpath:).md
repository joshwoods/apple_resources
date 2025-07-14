

- Foundation
- FileManager
-  attributesOfItem(atPath:) 

Instance Method

# attributesOfItem(atPath:)

Returns the attributes of the item at a given path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func attributesOfItem(atPath path: String) throws -> [FileAttributeKey : Any]
```

## Parameters 

`path`  

The path of a file or directory.

## Return Value

A dictionary object that describes the attributes (file, directory, symlink, and so on) of the file specified by `path` (or `nil` if an error occurred in Objective-C). The keys in the dictionary are described in `File Attribute Keys`.

## Discussion

If the item at the path is a symbolic link—that is, the value of the type key in the attributes dictionary is typeSymbolicLink—you can use the destinationOfSymbolicLink(atPath:) method to retrieve the path of the item pointed to by the link. You can also use the resolvingSymlinksInPath method of NSString to resolve links in the path before retrieving the item’s attributes.

As a convenience, NSDictionary provides a set of methods (declared as a category on NSDictionary) for quickly and efficiently obtaining attribute information from the returned dictionary: fileGroupOwnerAccountName(), fileModificationDate(), fileOwnerAccountName(), filePosixPermissions(), fileSize(), fileSystemFileNumber(), fileSystemNumber(), and fileType().

### Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Getting and Setting Attributes

func componentsToDisplay(forPath: String) -> [String]?

Returns an array of strings representing the user-visible components of a given path.

func displayName(atPath: String) -> String

Returns the display name of the file or directory at a specified path.

func attributesOfFileSystem(forPath: String) throws -> [FileAttributeKey : Any]

Returns a dictionary that describes the attributes of the mounted file system on which a given path resides.

func setAttributes([FileAttributeKey : Any], ofItemAtPath: String) throws

Sets the attributes of the specified file or directory.

