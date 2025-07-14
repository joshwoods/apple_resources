

- Foundation
- FileManager
-  attributesOfFileSystem(forPath:) 

Instance Method

# attributesOfFileSystem(forPath:)

Returns a dictionary that describes the attributes of the mounted file system on which a given path resides.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func attributesOfFileSystem(forPath path: String) throws -> [FileAttributeKey : Any]
```

## Parameters 

`path`  

Any pathname within the mounted file system.

## Return Value

A dictionary object that describes the attributes of the mounted file system on which `path` resides. See `File-System Attribute Keys` for a description of the keys available in the dictionary.

## Mentioned in 

About Apple File System

## Discussion

This method does not traverse a terminal symbolic link.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Getting and Setting Attributes

func componentsToDisplay(forPath: String) -> [String]?

Returns an array of strings representing the user-visible components of a given path.

func displayName(atPath: String) -> String

Returns the display name of the file or directory at a specified path.

func attributesOfItem(atPath: String) throws -> [FileAttributeKey : Any]

Returns the attributes of the item at a given path.

func setAttributes([FileAttributeKey : Any], ofItemAtPath: String) throws

Sets the attributes of the specified file or directory.

