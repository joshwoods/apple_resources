

- Foundation
- DistributedNotificationCenter
-  addObserver(\_:selector:name:object:suspensionBehavior:) 

Instance Method

# addObserver(\_:selector:name:object:suspensionBehavior:)

Adds an entry to the receiver’s dispatch table with a specific observer and suspended-notifications behavior, and optional notification name and sender.

Mac Catalyst 13.0+macOS 10.0+

``` source
func addObserver(
    _ observer: Any,
    selector: Selector,
    name: NSNotification.Name?,
    object: String?,
    suspensionBehavior: DistributedNotificationCenter.SuspensionBehavior
)
```

## Parameters 

`observer`  

Object registering as an observer. Must not be `nil`.

`selector`  

Selector that specifies the message the receiver sends `notificationObserver` to notify it of the notification posting. Must not be `0`.

`name`  

The name of the notification for which to register the observer; that is, only notifications with this name are delivered to the observer. When `nil`, the notification center doesn’t use a notification’s name to decide whether to deliver it to the observer.

`object`  

The object whose notifications the observer wants to receive; that is, only notifications sent by this sender are delivered to the observer. When `nil`, the notification center doesn’t use a notification’s sender to decide whether to deliver it to the observer.

`suspensionBehavior`  

Notification posting behavior when notification delivery is suspended.

## Discussion

The receiver does not retain `notificationObserver`. Therefore, you should always send removeObserver(_:) or removeObserver(_:name:object:) to the receiver before releasing `notificationObserver`.

## See Also

### Related Documentation

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, deliverImmediately: Bool)

Creates a notification with information and an immediate-delivery specifier, and posts it to the receiver.

### Managing Observers

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: String?)

Adds an entry to the notification center’s dispatch table with an observer, a selector, and an optional notification name and sender.

func removeObserver(Any, name: NSNotification.Name?, object: String?)

Removes matching entries from the receiver’s dispatch table.

