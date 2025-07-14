

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldProceedAfterError:linkingItemAt:to:) 

Instance Method

# fileManager(\_:shouldProceedAfterError:linkingItemAt:to:)

Asks the delegate if the operation should continue after an error occurs while linking to the item at the specified URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldProceedAfterError error: any Error,
    linkingItemAt srcURL: URL,
    to dstURL: URL
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that attempted to create the link.

`error`  

The error that occurred during the link attempt.

`srcURL`  

The URL of the attempted link location.

`dstURL`  

The URL of the file or directory that was the destination of the hard link.

## Return Value

true if the operation should proceed or false if it should be aborted. If you do not implement this method, the file manager assumes a response of false.

## Discussion

The file manager calls this method when there is a problem creating a hard link to the item at the specified location. If you return true, the file manager continues creating any other links associated with the current operation and ignores the error.

This method performs the same task as the fileManager(_:shouldProceedAfterError:linkingItemAtPath:toPath:) method and is preferred over that method in macOS 10.6 and later.

## See Also

### Related Documentation

func linkItem(at: URL, to: URL) throws

Creates a hard link between the items at the specified URLs.

func linkItem(atPath: String, toPath: String) throws

Creates a hard link between the items at the specified paths.

### Linking an Item

func fileManager(FileManager, shouldLinkItemAt: URL, to: URL) -> Bool

Asks the delegate if a hard link should be created between the items at the two URLs.

func fileManager(FileManager, shouldLinkItemAtPath: String, toPath: String) -> Bool

Asks the delegate if a hard link should be created between the items at the two paths.

func fileManager(FileManager, shouldProceedAfterError: any Error, linkingItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the operation should continue after an error occurs while linking to the item at the specified path.

