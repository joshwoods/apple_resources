

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldLinkItemAt:to:) 

Instance Method

# fileManager(\_:shouldLinkItemAt:to:)

Asks the delegate if a hard link should be created between the items at the two URLs.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldLinkItemAt srcURL: URL,
    to dstURL: URL
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that is attempting to create the link.

`srcURL`  

The URL identifying the new hard link to be created.

`dstURL`  

The URL identifying the destination of the link.

## Return Value

true if the link should be created or false if it should not be created.

## Discussion

If the item specified by `destURL` is a directory, returning false prevents links from being created to both the directory and its children.

This method performs the same task as the fileManager(_:shouldLinkItemAtPath:toPath:) method and is preferred over that method in macOS 10.6 and later.

## See Also

### Related Documentation

func linkItem(at: URL, to: URL) throws

Creates a hard link between the items at the specified URLs.

func linkItem(atPath: String, toPath: String) throws

Creates a hard link between the items at the specified paths.

### Linking an Item

func fileManager(FileManager, shouldLinkItemAtPath: String, toPath: String) -> Bool

Asks the delegate if a hard link should be created between the items at the two paths.

func fileManager(FileManager, shouldProceedAfterError: any Error, linkingItemAt: URL, to: URL) -> Bool

Asks the delegate if the operation should continue after an error occurs while linking to the item at the specified URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, linkingItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the operation should continue after an error occurs while linking to the item at the specified path.

