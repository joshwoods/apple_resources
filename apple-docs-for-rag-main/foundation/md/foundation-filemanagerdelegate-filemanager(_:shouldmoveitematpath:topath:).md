

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldMoveItemAtPath:toPath:) 

Instance Method

# fileManager(\_:shouldMoveItemAtPath:toPath:)

Asks the delegate if the file manager should move the specified item to the new path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldMoveItemAtPath srcPath: String,
    toPath dstPath: String
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that is attempting to move the file or directory.

`srcPath`  

The path to the file or directory that the file manager wants to move.

`dstPath`  

The new path for the file or directory.

## Return Value

true if the operation should proceed, otherwise false. If you do not implement this method, the file manager assumes a response of true.

## Discussion

This method is called only once for the item being moved, regardless of whether the item is a file, directory, or symbolic link.

This method performs the same task as the fileManager(_:shouldMoveItemAt:to:) method, which is preferred over this method in macOS 10.6 and later.

## See Also

### Related Documentation

func moveItem(atPath: String, toPath: String) throws

Moves the file or directory at the specified path to a new location synchronously.

func moveItem(at: URL, to: URL) throws

Moves the file or directory at the specified URL to a new location synchronously.

### Moving an Item

func fileManager(FileManager, shouldMoveItemAt: URL, to: URL) -> Bool

Asks the delegate if the file manager should move the specified item to the new URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, movingItemAt: URL, to: URL) -> Bool

Asks the delegate if the move operation should continue after an error occurs while moving the item at the specified URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, movingItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the move operation should continue after an error occurs while moving the item at the specified path.

