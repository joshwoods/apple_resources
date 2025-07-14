

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldProceedAfterError:copyingItemAt:to:) 

Instance Method

# fileManager(\_:shouldProceedAfterError:copyingItemAt:to:)

Asks the delegate if the move operation should continue after an error occurs while copying the item at the specified URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldProceedAfterError error: any Error,
    copyingItemAt srcURL: URL,
    to dstURL: URL
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that attempted to copy the item.

`error`  

The error that occurred during the attempt to copy.

`srcURL`  

The URL or a file or directory that `fileManager` is attempting to copy.

`dstURL`  

The URL or a file or directory to which `fileManager` is attempting to copy.

## Return Value

true if the operation should proceed or false if it should be aborted. If you do not implement this method, the file manager assumes a response of false.

## Discussion

The file manager calls this method when there is a problem copying the item to the specified location. If you return true, the file manager continues copying any other items and ignores the error.

This method performs the same task as the fileManager(_:shouldProceedAfterError:copyingItemAtPath:toPath:) method and is preferred over that method in macOS 10.6 and later.

## See Also

### Related Documentation

func copyItem(atPath: String, toPath: String) throws

Copies the item at the specified path to a new location synchronously.

func copyItem(at: URL, to: URL) throws

Copies the file at the specified URL to a new location synchronously.

### Copying an Item

func fileManager(FileManager, shouldCopyItemAt: URL, to: URL) -> Bool

Asks the delegate if the file manager should copy the specified item to the new URL.

func fileManager(FileManager, shouldCopyItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the file manager should copy the specified item to the new path.

func fileManager(FileManager, shouldProceedAfterError: any Error, copyingItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the move operation should continue after an error occurs while copying the item at the specified path.

