

- Foundation
-  DistributedNotificationCenter 

Class

# DistributedNotificationCenter

A notification dispatch mechanism that enables the broadcast of notifications across task boundaries.

Mac Catalyst 13.0+macOS 10.0+

``` source
class DistributedNotificationCenter
```

## Overview

A DistributedNotificationCenter instance broadcasts NSNotification objects to objects in other tasks that have registered for the notification with their task’s default distributed notification center.

### Principal Attributes

- Notification dispatch table. See “Class at a Glance” \> “Principal Attributes” in NotificationCenter for information about the dispatch table.

In addition to the notification name and sender, dispatch table entries for distributed notification centers specify when the notification center delivers notifications to its observers. See the postNotificationName(_:object:userInfo:deliverImmediately:) method, Suspending and Resuming Notification Delivery, and DistributedNotificationCenter.SuspensionBehavior for details.

### Commonly Used Methods

default()  
Accesses the default distributed notification center.

addObserver(_:selector:name:object:suspensionBehavior:)  
Registers an object to receive a notification with a specified behavior when notification delivery is suspended.

postNotificationName(_:object:userInfo:deliverImmediately:)  
Creates and posts a notification.

removeObserver(_:name:object:)  
Specifies that an object no longer wants to receive certain notifications.

### Overview

Each task has a default distributed notification center that you access with the default() class method. There may be different types of distributed notification centers. Currently there is a single type—`NSLocalNotificationCenterType`. This type of distributed notification center handles notifications that can be sent between tasks on a single computer. For communication between tasks on different computers, use Distributed Objects Programming Topics.

Posting a *distributed notification* is an expensive operation. The notification gets sent to a system-wide server that distributes it to all the tasks that have objects registered for distributed notifications. The latency between posting the notification and the notification’s arrival in another task is unbounded. In fact, when too many notifications are posted and the server’s queue fills up, notifications may be dropped.

Distributed notifications are delivered via a task’s run loop. A task must be running a run loop in one of the “common” modes, such as `NSDefaultRunLoopMode`, to receive a distributed notification. For multithreaded applications running in macOS 10.3 and later, distributed notifications are always delivered to the main thread. For multithreaded applications running in OS X v10.2.8 and earlier, notifications are delivered to the thread that first used the distributed notifications API, which in most cases is the main thread.

Important

`NSDistributedNotificationCenter` does not implement a secure communications protocol. When using distributed notifications, your app should treat any data passed in the notification as untrusted. See Security Overview for general guidance on secure coding practices.

Note

`NSDistributedNotificationCenter` objects should not be used to send notifications between threads within the same task. Use Distributed Objects Programming Topics or the NSObject method performSelector(onMainThread:with:waitUntilDone:), instead. You can also setup an Port object to receive and distribute messages from other threads.

## Topics

### Getting Distributed Notification Centers

class func `default`() -> DistributedNotificationCenter

Returns the default distributed notification center, representing the local notification center for the computer.

class func forType(DistributedNotificationCenter.CenterType) -> DistributedNotificationCenter

Returns the distributed notification center for a particular notification center type.

### Managing Observers

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: String?)

Adds an entry to the notification center’s dispatch table with an observer, a selector, and an optional notification name and sender.

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: String?, suspensionBehavior: DistributedNotificationCenter.SuspensionBehavior)

Adds an entry to the receiver’s dispatch table with a specific observer and suspended-notifications behavior, and optional notification name and sender.

func removeObserver(Any, name: NSNotification.Name?, object: String?)

Removes matching entries from the receiver’s dispatch table.

### Posting Notifications

func post(name: NSNotification.Name, object: String?)

Creates a notification, and posts it to the receiver.

func post(name: NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?)

Creates a notification with information, and posts it to the receiver.

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, deliverImmediately: Bool)

Creates a notification with information and an immediate-delivery specifier, and posts it to the receiver.

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, options: DistributedNotificationCenter.Options)

Creates a notification with information, and posts it to the receiver.

### Suspending and Resuming Notification Delivery

var suspended: Bool

Suspends or resumes notification delivery.

### Constants

struct Options

These constants specify the behavior of notifications posted using the postNotificationName(_:object:userInfo:options:) method.

struct CenterType

This constant specifies the notification center type.

enum SuspensionBehavior

These constants specify the types of notification delivery suspension behaviors.

## Relationships

### Inherits From

- NotificationCenter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

