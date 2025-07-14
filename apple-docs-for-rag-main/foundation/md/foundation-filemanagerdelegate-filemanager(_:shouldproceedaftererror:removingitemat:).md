

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldProceedAfterError:removingItemAt:) 

Instance Method

# fileManager(\_:shouldProceedAfterError:removingItemAt:)

Asks the delegate if the operation should continue after an error occurs while removing the item at the specified URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldProceedAfterError error: any Error,
    removingItemAt URL: URL
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that attempted to remove the item.

`error`  

The error that occurred while attempting to remove the item at `URL`.

`URL`  

The URL for the file or directory that the file manager tried to delete.

## Return Value

true if the operation should proceed or false if it should be aborted. If you do not implement this method, the file manager assumes a response of false.

## Discussion

The file manager calls this method when there is a problem deleting the item to the specified location. If you return true, the file manager continues deleting any remaining items and ignores the error.

This method performs the same task as the fileManager(_:shouldProceedAfterError:removingItemAtPath:) method and is preferred over that method in macOS 10.6 and later.

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

func fileManager(FileManager, shouldProceedAfterError: any Error, removingItemAtPath: String) -> Bool

Asks the delegate if the operation should continue after an error occurs while removing the item at the specified path.

