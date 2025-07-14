

- Foundation
- NSNotification
- NSNotification.Name
-  NSDidBecomeSingleThreaded 

Type Property

# NSDidBecomeSingleThreaded

Not implemented.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let NSDidBecomeSingleThreaded: NSNotification.Name
```

## See Also

### Notifications

static let NSThreadWillExit: NSNotification.Name

An `NSThread` object posts this notification when it receives the exit() message, before the thread exits. Observer methods invoked to receive this notification execute in the exiting thread, before it exits.

static let NSWillBecomeMultiThreaded: NSNotification.Name

Posted when the first thread is detached from the current thread. The `NSThread` class posts this notification at most once—the first time a thread is detached using detachNewThreadSelector(_:toTarget:with:) or the start() method. Subsequent invocations of those methods do not post this notification. Observers of this notification have their notification method invoked in the main thread, not the new thread. The observer notification methods always execute before the new thread begins executing.

