

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldCopyItemAt:to:) 

Instance Method

# fileManager(\_:shouldCopyItemAt:to:)

Asks the delegate if the file manager should copy the specified item to the new URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldCopyItemAt srcURL: URL,
    to dstURL: URL
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that is attempting to copy the file or directory.

`srcURL`  

The URL of the file or directory that the file manager wants to copy.

`dstURL`  

The URL specifying the location for the copied file or directory.

## Return Value

true if the item should be copied or false if the file manager should stop copying items associated with the current operation. If you do not implement this method, the file manager assumes a response of true.

## Discussion

This method is called once for each item that needs to be copied. Thus, for a directory, this method is called once for the directory and once for each item in the directory.

This method performs the same task as the fileManager(_:shouldCopyItemAtPath:toPath:) method and is preferred over that method in macOS 10.6 and later.

## See Also

### Related Documentation

func copyItem(atPath: String, toPath: String) throws

Copies the item at the specified path to a new location synchronously.

func copyItem(at: URL, to: URL) throws

Copies the file at the specified URL to a new location synchronously.

### Copying an Item

func fileManager(FileManager, shouldCopyItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the file manager should copy the specified item to the new path.

func fileManager(FileManager, shouldProceedAfterError: any Error, copyingItemAt: URL, to: URL) -> Bool

Asks the delegate if the move operation should continue after an error occurs while copying the item at the specified URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, copyingItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the move operation should continue after an error occurs while copying the item at the specified path.

