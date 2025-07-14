

- Foundation
- FileManager
-  getRelationship(\_:ofDirectoryAt:toItemAt:) 

Instance Method

# getRelationship(\_:ofDirectoryAt:toItemAt:)

Determines the type of relationship that exists between a directory and an item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getRelationship(
    _ outRelationship: UnsafeMutablePointer,
    ofDirectoryAt directoryURL: URL,
    toItemAt otherURL: URL
) throws
```

## Parameters 

`outRelationship`  

A pointer to a variable in which to put the relationship between `directoryURL` and `otherURL`. For a list of possible values, see FileManager.URLRelationship.

`directoryURL`  

The URL of the directory that potentially contains the item in `otherURL`. The URL in this parameter must specify a directory. This parameter must not be `nil`.

`otherURL`  

The URL of the file or directory whose relationship to `directoryURL` is being tested. This parameter must not be `nil`.

## Discussion

Use this method to determine the relationship between an item and a directory whose location you already know. If the relationship between the items is determined successfully, this method sets the value of the `outRelationship` parameter to an appropriate value. The directory may contain the item, it may be the same as the item, or it may not have a direct relationship to the item.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Getting the Relationship Between Items

func getRelationship(UnsafeMutablePointer&lt;FileManager.URLRelationship>, of: FileManager.SearchPathDirectory, in: FileManager.SearchPathDomainMask, toItemAt: URL) throws

Determines the type of relationship that exists between a system directory and the specified item.

enum URLRelationship

Constants indicating the relationship between a directory and an item.

