

- Foundation
- NotificationQueue
-  dequeueNotifications(matching:coalesceMask:) 

Instance Method

# dequeueNotifications(matching:coalesceMask:)

Removes all notifications from the queue that match a provided notification using provided matching criteria.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dequeueNotifications(
    matching notification: Notification,
    coalesceMask: Int
)
```

## Parameters 

`notification`  

The notification used for matching notifications to remove from the notification queue.

`coalesceMask`  

A mask indicating what criteria to use when matching attributes of `notification` to attributes of notifications in the queue. The mask is created by combining any of the constants none, onName, and onSender.

## See Also

### Managing Notifications

func enqueue(Notification, postingStyle: NotificationQueue.PostingStyle, coalesceMask: NotificationQueue.NotificationCoalescing, forModes: [RunLoop.Mode]?)

Adds a notification to the notification queue with a specified posting style, criteria for coalescing, and run loop mode.

func enqueue(Notification, postingStyle: NotificationQueue.PostingStyle)

Adds a notification to the notification queue with a specified posting style.

