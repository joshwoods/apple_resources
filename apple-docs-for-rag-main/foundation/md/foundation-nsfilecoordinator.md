

- Foundation
-  NSFileCoordinator 

Class

# NSFileCoordinator

An object that coordinates the reading and writing of files and directories among file presenters.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSFileCoordinator
```

## Mentioned in 

Improving performance and stability when accessing the file system

## Overview

The NSFileCoordinator class coordinates the reading and writing of files and directories among multiple processes and objects in the same process. You use instances of this class as is to read from, write to, modify the attributes of, change the location of, or delete a file or directory, but before your code to perform those actions executes, the file coordinator lets registered file presenter objects perform any tasks that they might require to ensure their own integrity. For example, if you want to change the location of a file, other objects interested in that file need to know where you intend to move it so that they can update their references.

Objects that adopt the NSFilePresenter protocol must register themselves with the NSFileCoordinator class to be notified of any pending changes. They do this by calling the addFilePresenter(_:) class method. A file presenter must balance calls to addFilePresenter(_:) with a call to removeFilePresenter(_:) before being released, even in a garbage-collected application. The file presenter class maintains a list of active file presenter objects in the current application and uses that list, plus the file coordinator classes in other processes, to deliver notifications to all of the objects interested in a particular item.

Instances of NSFileCoordinator are meant to be used on a per-file-operation basis, where a file operation is something like opening and reading the contents of a file or moving a batch of files and directories to a new location. There is no benefit to keeping a file coordinator object past the length of the planned operation. In fact, because file coordinators retain file presenter objects, keeping one around could prevent the file presenter objects from being released in a timely manner.

For information about implementing a file presenter object to receive file-related notifications, see NSFilePresenter.

### File Presenters and iOS

If your app or extension enters the background with an active file presenter, it may be terminated by the system in order to prevent deadlock on that file. To prevent this situation, call removeFilePresenter(_:) to remove the file presenter in the applicationDidEnterBackground(_:) method or in response to a didEnterBackgroundNotification notification. Call addFilePresenter(_:) to add the file presenter again in the applicationWillEnterForeground(_:) method or in response to a willEnterForegroundNotification notification.

Note

The UIDocument class automatically removes itself when your app goes to the background. It automatically adds itself again when your app returns to the foreground.

### File Coordinators and iOS

A coordinated read or write will automatically begin a background task when granted, similar to one created with the beginBackgroundTask(expirationHandler:) method. This helps ensure that your app or extension has sufficient time to finish the read or write operation if it’s suspended, without creating a deadlock on access to that file by other processes. If a process is suspended while waiting for a coordinated read or write to be granted, the request is canceled, and an `NSError` object with the code NSUserCancelledError is produced. If the background task expires, the process is terminated.

Note

The UIDocument class automatically requests additional background time and safely performs coordinated reads and writes when loading and saving the document.

### Threading Considerations

Each file coordinator object you create should be used on a single thread only. If you need to coordinate file operations across multiple objects in different threads, each object should create its own file coordinator.

## Topics

### Initializing a File Coordinator

init(filePresenter: (any NSFilePresenter)?)

Initializes and returns a file coordinator object using the specified file presenter.

### Managing File Presenters

class func addFilePresenter(any NSFilePresenter)

Registers the specified file presenter object so that it can receive notifications.

class func removeFilePresenter(any NSFilePresenter)

Unregisters the specified file presenter object.

class var filePresenters: [any NSFilePresenter]

Returns an array containing the currently registered file presenter objects.

var purposeIdentifier: String

A string that uniquely identifies the file access that was performed by this file coordinator.

### Coordinating File Operations Asynchronously

func coordinate(with: [NSFileAccessIntent], queue: OperationQueue, byAccessor: ((any Error)?) -> Void)

Performs a number of coordinated-read or -write operations asynchronously.

### Coordinating File Operations Synchronously

func coordinate(readingItemAt: URL, options: NSFileCoordinator.ReadingOptions, error: NSErrorPointer, byAccessor: (URL) -> Void)

Initiates a read operation on a single file or directory using the specified options.

func coordinate(writingItemAt: URL, options: NSFileCoordinator.WritingOptions, error: NSErrorPointer, byAccessor: (URL) -> Void)

Initiates a write operation on a single file or directory using the specified options.

func coordinate(readingItemAt: URL, options: NSFileCoordinator.ReadingOptions, writingItemAt: URL, options: NSFileCoordinator.WritingOptions, error: NSErrorPointer, byAccessor: (URL, URL) -> Void)

Initiates a read operation that contains a follow-up write operation.

func coordinate(writingItemAt: URL, options: NSFileCoordinator.WritingOptions, writingItemAt: URL, options: NSFileCoordinator.WritingOptions, error: NSErrorPointer, byAccessor: (URL, URL) -> Void)

Initiates a write operation that involves a secondary write operation.

func prepare(forReadingItemsAt: [URL], options: NSFileCoordinator.ReadingOptions, writingItemsAt: [URL], options: NSFileCoordinator.WritingOptions, error: NSErrorPointer, byAccessor: (() -> Void) -> Void)

Prepare to read or write from multiple files in a single batch operation.

func item(at: URL, willMoveTo: URL)

Announces that your app is moving a file to a new URL.

func item(at: URL, didMoveTo: URL)

Notifies relevant file presenters that the location of a file or directory changed.

func cancel()

Cancels any active file coordination calls.

### Constants

struct ReadingOptions

Options to use when reading the contents or attributes of a file or directory.

struct WritingOptions

Options to use when changing the contents or attributes of a file or directory.

### Ubiquity Change Notifications

func item(at: URL, didChangeUbiquityAttributes: Set&lt;URLResourceKey>)

Tells observing file providers that the item’s ubiquity attributes have changed.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Coordinated file access

protocol NSFilePresenter

The interface a file coordinator uses to inform an object presenting a file about changes to that file made elsewhere in the system.

class NSFileAccessIntent

The details of a coordinated-read or coordinated-write operation.

