

- Foundation
-  NSFilePresenter 

Protocol

# NSFilePresenter

The interface a file coordinator uses to inform an object presenting a file about changes to that file made elsewhere in the system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSFilePresenter : NSObjectProtocol
```

## Mentioned in 

Improving performance and stability when accessing the file system

## Overview

Objects that allow the user to view or edit the content of files or directories should adopt the NSFilePresenter protocol. You use file presenters in conjunction with an NSFileCoordinator object to coordinate access to a file or directory among the objects of your application and between your application and other processes. When changes to an item occur, the system notifies objects that adopt this protocol and gives them a chance to respond appropriately.

Use the methods of this protocol to respond to actions about to be taken on the presented file or directory. When another object or process uses a file coordinator to begin reading or writing a file or directory, the file coordinator notifies all presented objects interested in the item first. It notifies the presenter objects by invoking one of the methods defined by this protocol on that object. The actual invocation of that method occurs on the operation queue in the presentedItemOperationQueue property. Your file presenter must provide this queue. If your queue supports the concurrent execution of operations, the methods of your presenter object must be thread-safe and able to run in multiple queues simultaneously.

You can use file presenters to coordinate access to a file or directory among your application’s objects. If another process uses a file coordinator for the same file or directory, your presenter objects are similarly notified whenever the other process makes its changes. Your presenter objects are not notified about changes made directly using low-level read and write calls to the file. Only changes that go through a file coordinator result in notifications.

For information about how to use file presenters with a file coordinator object, see NSFileCoordinator.

### File Presenters and iOS

If your app enters the background with an active file presenter, any other processes that perform a coordinated read or write on the presented file can deadlock. To prevent this situation, call the coordinator’s removeFilePresenter(_:) type method to remove the file presenter in the applicationDidEnterBackground(_:) method or in response to a didEnterBackgroundNotification notification. Call addFilePresenter(_:) to add the file presenter again in the applicationWillEnterForeground(_:) method or in response to a willEnterForegroundNotification notification.

Note

The UIDocument class automatically removes itself when your app goes to the background. It automatically adds itself again when your app returns to the foreground.

## Topics

### Accessing File Presenter Attributes

var presentedItemURL: URL?

The URL of the presented file or directory.

**Required**

var presentedItemOperationQueue: OperationQueue

The operation queue in which to execute presenter-related messages.

**Required**

var primaryPresentedItemURL: URL?

The URL of a secondary item’s primary presented file or directory.

### Relinquishing Managed Files

func relinquishPresentedItem(toReader: ((() -> Void)?) -> Void)

Notifies your object that another object or process wants to read the presented file or directory.

func relinquishPresentedItem(toWriter: ((() -> Void)?) -> Void)

Notifies your object that another object or process wants to write to the presented file or directory.

### Handling Changes to Files

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

Tells your object to save any unsaved changes for the presented item.

func accommodatePresentedItemDeletion(completionHandler: ((any Error)?) -> Void)

Tells your object that its presented item is about to be deleted.

func presentedItemDidMove(to: URL)

Tells your object that the presented item moved or was renamed.

func presentedItemDidChange()

Tells your object that the presented item’s contents or attributes changed.

### Responding to Version Changes

func presentedItemDidGain(NSFileVersion)

Tells the delegate that a new version of the file or file package was added.

func presentedItemDidLose(NSFileVersion)

Tells the delegate that a version of the file or file package was removed.

func presentedItemDidResolveConflict(NSFileVersion)

Tells the delegate that some other entity resolved a version conflict for the presenter’s file or file package.

func presentedSubitem(at: URL, didGain: NSFileVersion)

Tells the delegate that the item inside the presented directory gained a new version.

func presentedSubitem(at: URL, didLose: NSFileVersion)

Tells the delegate that the item inside the presented directory lost an existing version.

func presentedSubitem(at: URL, didResolve: NSFileVersion)

Tells the delegate that the item inside the presented directory had a version conflict resolved by an outside entity.

### Handling Changes to a Presented Directory

func accommodatePresentedSubitemDeletion(at: URL, completionHandler: ((any Error)?) -> Void)

Tells the delegate that some entity wants to delete an item that is inside of a presented directory.

func presentedSubitemDidAppear(at: URL)

Tells the delegate that an item was added to the presented directory.

func presentedSubitem(at: URL, didMoveTo: URL)

Tells the delegate that an item in the presented directory moved to a new location.

func presentedSubitemDidChange(at: URL)

Tells the delegate that the contents or attributes of the specified item changed.

### Ubiquity Change Notifications

var observedPresentedItemUbiquityAttributes: Set&lt;URLResourceKey>

A list of ubiquity attributes used to generate and send notifications whenever an attribute in the list changes.

func presentedItemDidChangeUbiquityAttributes(Set&lt;URLResourceKey>)

Tells your object that the file or file package’s ubiquity attributes have changed.

### Instance Methods

func accommodatePresentedItemEviction(completionHandler: ((any Error)?) -> Void)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Coordinated file access

class NSFileAccessIntent

The details of a coordinated-read or coordinated-write operation.

class NSFileCoordinator

An object that coordinates the reading and writing of files and directories among file presenters.

