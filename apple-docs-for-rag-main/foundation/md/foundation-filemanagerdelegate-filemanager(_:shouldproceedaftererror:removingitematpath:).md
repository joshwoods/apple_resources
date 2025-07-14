

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldProceedAfterError:removingItemAtPath:) 

Instance Method

# fileManager(\_:shouldProceedAfterError:removingItemAtPath:)

Asks the delegate if the operation should continue after an error occurs while removing the item at the specified path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldProceedAfterError error: any Error,
    removingItemAtPath path: String
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that attempted to remove the item.

`error`  

The error that occurred during the attempt to copy.

`path`  

The path for the file or directory that the file manager tried to delete.

## Return Value

true if the operation should proceed or false if it should be aborted. If you do not implement this method, the file manager assumes a response of false.

## Discussion

The file manager calls this method when there is a problem deleting the item to the specified location. If you return true, the file manager continues deleting any remaining items and ignores the error.

This method performs the same task as the fileManager(_:shouldProceedAfterError:removingItemAt:) method, which is preferred over this method in macOS 10.6 and later.

## See Also

### Related Documentation

func removeItem(atPath: String) throws

Removes the file or directory at the specified path.

func removeItem(at: URL) throws

Removes the file or directory at the specified URL.

### Removing an Item

func fileManager(FileManager, shouldRemoveItemAt: URL) -> Bool

Asks the delegate whether the item at the specified URL should be deleted.

func fileManager(FileManager, shouldRemoveItemAtPath: String) -> Bool

Asks the delegate whether the item at the specified path should be deleted.

func fileManager(FileManager, shouldProceedAfterError: any Error, removingItemAt: URL) -> Bool

Asks the delegate if the operation should continue after an error occurs while removing the item at the specified URL.

