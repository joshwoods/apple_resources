

- Foundation
- FileManager
-  moveItem(atPath:toPath:) 

Instance Method

# moveItem(atPath:toPath:)

Moves the file or directory at the specified path to a new location synchronously.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func moveItem(
    atPath srcPath: String,
    toPath dstPath: String
) throws
```

## Parameters 

`srcPath`  

The path to the file or directory you want to move. This parameter must not be `nil`.

`dstPath`  

The new path for the item in `srcPath`. This path must include the name of the file or directory in its new location. This parameter must not be `nil`.

## Discussion

When moving items, the current process must have permission to read the item at `srcPath` and write the parent directory of `dstPath`. If the item at `srcPath` is a directory, this method moves the directory and all of its contents, including any hidden files. If an item with the same name already exists at `dstPath`, this method stops the move attempt and returns an appropriate error. If the last component of `srcPath` is a symbolic link, only the link is moved to the new path; the item pointed to by the link remains at its current location.

Prior to moving the item, the file manager asks its delegate if it should actually move it. It does this by calling the fileManager(_:shouldMoveItemAt:to:) method; if that method is not implemented it calls the fileManager(_:shouldMoveItemAtPath:toPath:) method instead. If the item being moved is a directory, the file manager notifies the delegate only for the directory itself and not for any of its contents. If the delegate method returns true, or if the delegate does not implement the appropriate methods, the file manager moves the file. If there is an error moving one out of several items, the file manager may also call the delegate’s fileManager(_:shouldProceedAfterError:movingItemAt:to:) or fileManager(_:shouldProceedAfterError:movingItemAtPath:toPath:) method to determine how to proceed.

If the source and destination of the move operation are not on the same volume, this method copies the item first and then removes it from its current location. This behavior may trigger additional delegate notifications related to copying and removing individual items.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func removeItem(atPath: String) throws

Removes the file or directory at the specified path.

### Moving and Copying Items

func copyItem(at: URL, to: URL) throws

Copies the file at the specified URL to a new location synchronously.

func copyItem(atPath: String, toPath: String) throws

Copies the item at the specified path to a new location synchronously.

func moveItem(at: URL, to: URL) throws

Moves the file or directory at the specified URL to a new location synchronously.

