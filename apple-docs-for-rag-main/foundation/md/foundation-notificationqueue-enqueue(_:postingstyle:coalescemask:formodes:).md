

- Foundation
- NotificationQueue
-  enqueue(\_:postingStyle:coalesceMask:forModes:) 

Instance Method

# enqueue(\_:postingStyle:coalesceMask:forModes:)

Adds a notification to the notification queue with a specified posting style, criteria for coalescing, and run loop mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enqueue(
    _ notification: Notification,
    postingStyle: NotificationQueue.PostingStyle,
    coalesceMask: NotificationQueue.NotificationCoalescing,
    forModes modes: [RunLoop.Mode]?
)
```

## Parameters 

`notification`  

The notification to add to the queue.

`postingStyle`  

The posting style for the notification. The posting style indicates when the notification queue should post the notification to its notification center.

`coalesceMask`  

A mask indicating what criteria to use when matching attributes of `notification` to attributes of notifications in the queue. The mask is created by combining any of the constants none, onName, and onSender.

`modes`  

The list of modes the notification may be posted in. The notification queue will only post the notification to its notification center if the run loop is in one of the modes provided in the array.

This parameter may be `nil`, in which case it defaults to default.

## See Also

### Managing Notifications

func enqueue(Notification, postingStyle: NotificationQueue.PostingStyle)

Adds a notification to the notification queue with a specified posting style.

func dequeueNotifications(matching: Notification, coalesceMask: Int)

Removes all notifications from the queue that match a provided notification using provided matching criteria.

