

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldProceedAfterError:movingItemAtPath:toPath:) 

Instance Method

# fileManager(\_:shouldProceedAfterError:movingItemAtPath:toPath:)

Asks the delegate if the move operation should continue after an error occurs while moving the item at the specified path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldProceedAfterError error: any Error,
    movingItemAtPath srcPath: String,
    toPath dstPath: String
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that attempted to move the item.

`error`  

The error that occurred while trying to move the item in `srcPath`.

`srcPath`  

The path of the file or directory that the file manager tried to move.

`dstPath`  

The path of the intended destination for the item in `srcPath`.

## Return Value

true if the operation should proceed or false if it should be aborted. If you do not implement this method, the file manager assumes a response of false.

## Discussion

The file manager calls this method when there is a problem moving the item to the specified location. If you return true, the file manager proceeds to remove the item from its current location as if the move operation had completed successfully.

This method performs the same task as the fileManager(_:shouldProceedAfterError:movingItemAt:to:) method, which is preferred over this method in macOS 10.6 and later.

## See Also

### Related Documentation

func moveItem(atPath: String, toPath: String) throws

Moves the file or directory at the specified path to a new location synchronously.

func moveItem(at: URL, to: URL) throws

Moves the file or directory at the specified URL to a new location synchronously.

### Moving an Item

func fileManager(FileManager, shouldMoveItemAt: URL, to: URL) -> Bool

Asks the delegate if the file manager should move the specified item to the new URL.

func fileManager(FileManager, shouldMoveItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the file manager should move the specified item to the new path.

func fileManager(FileManager, shouldProceedAfterError: any Error, movingItemAt: URL, to: URL) -> Bool

Asks the delegate if the move operation should continue after an error occurs while moving the item at the specified URL.

