

- Foundation
- DistributedNotificationCenter
-  addObserver(\_:selector:name:object:) 

Instance Method

# addObserver(\_:selector:name:object:)

Adds an entry to the notification center’s dispatch table with an observer, a selector, and an optional notification name and sender.

Mac Catalyst 13.0+macOS 10.0+

``` source
func addObserver(
    _ observer: Any,
    selector aSelector: Selector,
    name aName: NSNotification.Name?,
    object anObject: String?
)
```

## Parameters 

`observer`  

An object registering as an observer.

`aSelector`  

A selector that the notification center sends `notificationObserver` to notify when posting the notification.

`aName`  

The name of the notification for which to register the observer; that is, only notifications with this name are delivered to the observer. When `nil`, the notification center doesn’t use a notification’s name to decide whether to deliver it to the observer.

`anObject`  

The object whose notifications the observer wants to receive; that is, only notifications sent by this sender are delivered to the observer. When `nil`, the notification center doesn’t use a notification’s sender to decide whether to deliver it to the observer.

## Discussion

This method calls addObserver(_:selector:name:object:suspensionBehavior:), passing DistributedNotificationCenter.SuspensionBehavior.coalesce for `suspensionBehavior`.

## See Also

### Managing Observers

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: String?, suspensionBehavior: DistributedNotificationCenter.SuspensionBehavior)

Adds an entry to the receiver’s dispatch table with a specific observer and suspended-notifications behavior, and optional notification name and sender.

func removeObserver(Any, name: NSNotification.Name?, object: String?)

Removes matching entries from the receiver’s dispatch table.

