

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldRemoveItemAtPath:) 

Instance Method

# fileManager(\_:shouldRemoveItemAtPath:)

Asks the delegate whether the item at the specified path should be deleted.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldRemoveItemAtPath path: String
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that is attempting to remove the file or directory.

`path`  

The path to the file or directory that the file manager is attempting to delete.

## Return Value

true if the specified item should be deleted or false if it should not be deleted.

## Discussion

Removed items are deleted immediately and not placed in the Trash. If the specified item is a directory, returning false prevents both the directory and its children from being deleted.

This method performs the same task as the fileManager(_:shouldRemoveItemAt:) method, which is preferred over this method in macOS 10.6 and later.

## See Also

### Related Documentation

func removeItem(atPath: String) throws

Removes the file or directory at the specified path.

func removeItem(at: URL) throws

Removes the file or directory at the specified URL.

### Removing an Item

func fileManager(FileManager, shouldRemoveItemAt: URL) -> Bool

Asks the delegate whether the item at the specified URL should be deleted.

func fileManager(FileManager, shouldProceedAfterError: any Error, removingItemAt: URL) -> Bool

Asks the delegate if the operation should continue after an error occurs while removing the item at the specified URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, removingItemAtPath: String) -> Bool

Asks the delegate if the operation should continue after an error occurs while removing the item at the specified path.

