

- Foundation
- FileManager
-  copyItem(atPath:toPath:) 

Instance Method

# copyItem(atPath:toPath:)

Copies the item at the specified path to a new location synchronously.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func copyItem(
    atPath srcPath: String,
    toPath dstPath: String
) throws
```

## Parameters 

`srcPath`  

The path to the file or directory you want to move. This parameter must not be `nil`.

`dstPath`  

The path at which to place the copy of `srcPath`. This path must include the name of the file or directory in its new location. This parameter must not be `nil`.

## Mentioned in 

About Apple File System

## Discussion

When copying items, the current process must have permission to read the file or directory at `srcPath` and write the parent directory of `dstPath`. If the item at `srcPath` is a directory, this method copies the directory and all of its contents, including any hidden files. If a file with the same name already exists at `dstPath`, this method stops the copy attempt and returns an appropriate error. If the last component of `srcPath` is a symbolic link, only the link is copied to the new path.

Prior to copying an item, the file manager asks its delegate if it should actually do so for each item. It does this by calling the fileManager(_:shouldCopyItemAt:to:) method; if that method is not implemented it calls the fileManager(_:shouldCopyItemAtPath:toPath:) method instead. If the delegate method returns true, or if the delegate does not implement the appropriate methods, the file manager copies the given file or directory. If there is an error copying an item, the file manager may also call the delegate’s fileManager(_:shouldProceedAfterError:copyingItemAt:to:) or fileManager(_:shouldProceedAfterError:copyingItemAtPath:toPath:) method to determine how to proceed.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Moving and Copying Items

func copyItem(at: URL, to: URL) throws

Copies the file at the specified URL to a new location synchronously.

func moveItem(at: URL, to: URL) throws

Moves the file or directory at the specified URL to a new location synchronously.

func moveItem(atPath: String, toPath: String) throws

Moves the file or directory at the specified path to a new location synchronously.

