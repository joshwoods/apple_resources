

- Foundation
- FileManager
-  createSymbolicLink(atPath:withDestinationPath:) 

Instance Method

# createSymbolicLink(atPath:withDestinationPath:)

Creates a symbolic link that points to the specified destination.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func createSymbolicLink(
    atPath path: String,
    withDestinationPath destPath: String
) throws
```

## Parameters 

`path`  

The path at which to create the new symbolic link. The last path component is used as the name of the link.

`destPath`  

The path that contains the item to be pointed to by the link. In other words, this is the destination of the link.

## Discussion

This method does not traverse symbolic links contained in `destPath`, making it possible to create symbolic links to locations that do not yet exist. Also, if the final path component in `path` is a symbolic link, that link is not followed.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func removeItem(atPath: String) throws

Removes the file or directory at the specified path.

### Creating Symbolic and Hard Links

func createSymbolicLink(at: URL, withDestinationURL: URL) throws

Creates a symbolic link at the specified URL that points to an item at the given URL.

func linkItem(at: URL, to: URL) throws

Creates a hard link between the items at the specified URLs.

func linkItem(atPath: String, toPath: String) throws

Creates a hard link between the items at the specified paths.

func destinationOfSymbolicLink(atPath: String) throws -> String

Returns the path of the item pointed to by a symbolic link.

