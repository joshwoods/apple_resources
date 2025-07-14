

- Foundation
- FileManager
-  linkItem(atPath:toPath:) 

Instance Method

# linkItem(atPath:toPath:)

Creates a hard link between the items at the specified paths.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func linkItem(
    atPath srcPath: String,
    toPath dstPath: String
) throws
```

## Parameters 

`srcPath`  

The path that specifies the item you wish to link to. The value in this parameter must not be `nil`.

`dstPath`  

The path that identifies the location where the link will be created. The value in this parameter must not be `nil`.

## Discussion

Use this method to create hard links between files in the current file system. If `srcPath` is a directory, this method creates a new directory at `dstPath` and then creates hard links for the items in that directory. If `srcPath` is (or contains) a symbolic link, the symbolic link is copied to the new location and not converted to a hard link.

Prior to linking each item, the file manager asks its delegate if it should actually create the link. It does this by calling the fileManager(_:shouldLinkItemAt:to:) method; if that method is not implemented it calls the fileManager(_:shouldLinkItemAtPath:toPath:) method instead. If the delegate method returns true, or if the delegate does not implement the appropriate methods, the file manager creates the hard link. If there is an error linking one out of several items, the file manager may also call the delegate’s fileManager(_:shouldProceedAfterError:linkingItemAt:to:) or fileManager(_:shouldProceedAfterError:linkingItemAtPath:toPath:) method to determine how to proceed.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating Symbolic and Hard Links

func createSymbolicLink(at: URL, withDestinationURL: URL) throws

Creates a symbolic link at the specified URL that points to an item at the given URL.

func createSymbolicLink(atPath: String, withDestinationPath: String) throws

Creates a symbolic link that points to the specified destination.

func linkItem(at: URL, to: URL) throws

Creates a hard link between the items at the specified URLs.

func destinationOfSymbolicLink(atPath: String) throws -> String

Returns the path of the item pointed to by a symbolic link.

