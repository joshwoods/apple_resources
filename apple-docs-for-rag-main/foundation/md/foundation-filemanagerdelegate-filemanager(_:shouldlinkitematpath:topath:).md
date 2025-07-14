

- Foundation
- FileManagerDelegate
-  fileManager(\_:shouldLinkItemAtPath:toPath:) 

Instance Method

# fileManager(\_:shouldLinkItemAtPath:toPath:)

Asks the delegate if a hard link should be created between the items at the two paths.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func fileManager(
    _ fileManager: FileManager,
    shouldLinkItemAtPath srcPath: String,
    toPath dstPath: String
) -> Bool
```

## Parameters 

`fileManager`  

The file manager object that is attempting to create the link.

`srcPath`  

The path or a file or directory that `fileManager` is about to attempt to link.

`dstPath`  

The path or a file or directory to which `fileManager` is about to attempt to link.

## Return Value

true if the operation should proceed, otherwise false.

## Discussion

If the item specified by `destURL` is a directory, returning false prevents links from being created to both the directory and its children.

This method performs the same task as the fileManager(_:shouldLinkItemAt:to:) method, which is preferred over this method in macOS 10.6 and later.

## See Also

### Related Documentation

func linkItem(at: URL, to: URL) throws

Creates a hard link between the items at the specified URLs.

func linkItem(atPath: String, toPath: String) throws

Creates a hard link between the items at the specified paths.

### Linking an Item

func fileManager(FileManager, shouldLinkItemAt: URL, to: URL) -> Bool

Asks the delegate if a hard link should be created between the items at the two URLs.

func fileManager(FileManager, shouldProceedAfterError: any Error, linkingItemAt: URL, to: URL) -> Bool

Asks the delegate if the operation should continue after an error occurs while linking to the item at the specified URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, linkingItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the operation should continue after an error occurs while linking to the item at the specified path.

