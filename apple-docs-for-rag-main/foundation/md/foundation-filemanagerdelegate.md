

- Foundation
-  FileManagerDelegate 

Protocol

# FileManagerDelegate

The interface a file manager’s delegate uses to intervene during operations or if an error occurs.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol FileManagerDelegate : NSObjectProtocol
```

## Overview

The FileManagerDelegate protocol defines optional methods for managing operations involving the copying, moving, linking, or removal of files and directories. When you use an FileManager object to initiate a copy, move, link, or remove operation, the file manager asks its delegate whether the operation should begin at all and whether it should proceed when an error occurs.

The methods of this protocol accept either NSURL or NSString objects. The file manager always prefers methods that take an NSURL object over those that take an NSString object.

You should associate your delegate with a unique instance of the FileManager class, as opposed to the shared instance.

## Topics

### Moving an Item

func fileManager(FileManager, shouldMoveItemAt: URL, to: URL) -> Bool

Asks the delegate if the file manager should move the specified item to the new URL.

func fileManager(FileManager, shouldMoveItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the file manager should move the specified item to the new path.

func fileManager(FileManager, shouldProceedAfterError: any Error, movingItemAt: URL, to: URL) -> Bool

Asks the delegate if the move operation should continue after an error occurs while moving the item at the specified URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, movingItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the move operation should continue after an error occurs while moving the item at the specified path.

### Copying an Item

func fileManager(FileManager, shouldCopyItemAt: URL, to: URL) -> Bool

Asks the delegate if the file manager should copy the specified item to the new URL.

func fileManager(FileManager, shouldCopyItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the file manager should copy the specified item to the new path.

func fileManager(FileManager, shouldProceedAfterError: any Error, copyingItemAt: URL, to: URL) -> Bool

Asks the delegate if the move operation should continue after an error occurs while copying the item at the specified URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, copyingItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the move operation should continue after an error occurs while copying the item at the specified path.

### Removing an Item

func fileManager(FileManager, shouldRemoveItemAt: URL) -> Bool

Asks the delegate whether the item at the specified URL should be deleted.

func fileManager(FileManager, shouldRemoveItemAtPath: String) -> Bool

Asks the delegate whether the item at the specified path should be deleted.

func fileManager(FileManager, shouldProceedAfterError: any Error, removingItemAt: URL) -> Bool

Asks the delegate if the operation should continue after an error occurs while removing the item at the specified URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, removingItemAtPath: String) -> Bool

Asks the delegate if the operation should continue after an error occurs while removing the item at the specified path.

### Linking an Item

func fileManager(FileManager, shouldLinkItemAt: URL, to: URL) -> Bool

Asks the delegate if a hard link should be created between the items at the two URLs.

func fileManager(FileManager, shouldLinkItemAtPath: String, toPath: String) -> Bool

Asks the delegate if a hard link should be created between the items at the two paths.

func fileManager(FileManager, shouldProceedAfterError: any Error, linkingItemAt: URL, to: URL) -> Bool

Asks the delegate if the operation should continue after an error occurs while linking to the item at the specified URL.

func fileManager(FileManager, shouldProceedAfterError: any Error, linkingItemAtPath: String, toPath: String) -> Bool

Asks the delegate if the operation should continue after an error occurs while linking to the item at the specified path.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### File system operations

Improving performance and stability when accessing the file system

Prevent data loss and app crashes by interacting with the file system in a coordinated, asynchronous manner and by avoiding unnecessary disk I/O.

class FileManager

A convenient interface to the contents of the file system, and the primary means of interacting with it.

About Apple File System

Use high-level APIs to get the most out of Apple File System.

