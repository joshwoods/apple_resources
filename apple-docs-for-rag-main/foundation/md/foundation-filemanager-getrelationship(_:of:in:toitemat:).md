

- Foundation
- FileManager
-  getRelationship(\_:of:in:toItemAt:) 

Instance Method

# getRelationship(\_:of:in:toItemAt:)

Determines the type of relationship that exists between a system directory and the specified item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getRelationship(
    _ outRelationship: UnsafeMutablePointer,
    of directory: FileManager.SearchPathDirectory,
    in domainMask: FileManager.SearchPathDomainMask,
    toItemAt url: URL
) throws
```

## Parameters 

`outRelationship`  

A pointer to a variable in which to put the relationship between `directoryURL` and `otherURL`. For a list of possible values, see FileManager.URLRelationship.

`directory`  

The search path directory. For a list of possible values, see FileManager.SearchPathDirectory.

`domainMask`  

The file system domain to search. Specify `0` for this parameter if you want the file manager to choose the domain that is most appropriate for the specified `url`.

`url`  

The URL of the file or directory whose relationship to `directoryURL` is being tested. This parameter must not be `nil`.

## Discussion

Use this method to determine the relationship between an item and one of the system-specific directories. For example, you might use this method to determine if the specified item is in the user’s `Documents` directory or is in the trash. If the relationship between the items is determined successfully, this method sets the value of the `outRelationship` parameter to an appropriate value. The directory may contain the item, it may be the same as the item, or it may not have a direct relationship to the item.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Getting the Relationship Between Items

func getRelationship(UnsafeMutablePointer&lt;FileManager.URLRelationship>, ofDirectoryAt: URL, toItemAt: URL) throws

Determines the type of relationship that exists between a directory and an item.

enum URLRelationship

Constants indicating the relationship between a directory and an item.

