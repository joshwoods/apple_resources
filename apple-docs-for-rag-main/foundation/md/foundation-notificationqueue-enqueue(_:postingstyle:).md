

- Foundation
- NotificationQueue
-  enqueue(\_:postingStyle:) 

Instance Method

# enqueue(\_:postingStyle:)

Adds a notification to the notification queue with a specified posting style.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enqueue(
    _ notification: Notification,
    postingStyle: NotificationQueue.PostingStyle
)
```

## Parameters 

`notification`  

The notification to add to the queue.

`postingStyle`  

The posting style for the notification. The posting style indicates when the notification queue should post the notification to its notification center.

## Discussion

This is a convenience method for calling enqueue(_:postingStyle:coalesceMask:forModes:) with coalescing criteria that will coalesce only notifications that match both the notification’s name and object and the runloop mode default.

## See Also

### Managing Notifications

func enqueue(Notification, postingStyle: NotificationQueue.PostingStyle, coalesceMask: NotificationQueue.NotificationCoalescing, forModes: [RunLoop.Mode]?)

Adds a notification to the notification queue with a specified posting style, criteria for coalescing, and run loop mode.

func dequeueNotifications(matching: Notification, coalesceMask: Int)

Removes all notifications from the queue that match a provided notification using provided matching criteria.

