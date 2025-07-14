

- Foundation
- NotificationCenter
-  addObserver(\_:selector:name:object:) 

Instance Method

# addObserver(\_:selector:name:object:)

Adds an entry to the notification center to call the provided selector with the notification.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addObserver(
    _ observer: Any,
    selector aSelector: Selector,
    name aName: NSNotification.Name?,
    object anObject: Any?
)
```

## Parameters 

`observer`  

An object to register as an observer.

`aSelector`  

A selector that specifies the message the receiver sends `observer` to alert it to the notification posting. The method that `aSelector` specifies must have one and only one argument (an instance of `NSNotification`).

`aName`  

The name of the notification to register for delivery to the observer. Specify a notification name to deliver only entries with this notification name.

When `nil`, the sender doesn’t use notification names as criteria for the delivery.

`anObject`  

The object that sends notifications to the observer. Specify a notification sender to deliver only notifications from this sender.

When `nil`, the notification center doesn’t use sender names as criteria for delivery.

## Discussion

Unregister an observer to stop receiving notifications.

To unregister an observer, use removeObserver(_:) or removeObserver(_:name:object:) with the most specific detail possible. For example, if you used a name and object to register the observer, use the name and object to remove it.

If your app targets iOS 9.0 and later or macOS 10.11 and later, you do not need to unregister an observer that you created with this function. If you forget or are unable to remove an observer, the system cleans up the next time it would have posted to it.

## See Also

### Adding and Removing Notification Observers

func addObserver(forName: NSNotification.Name?, object: Any?, queue: OperationQueue?, using: (Notification) -> Void) -> any NSObjectProtocol

Adds an entry to the notification center to receive notifications that passed to the provided block.

func removeObserver(Any, name: NSNotification.Name?, object: Any?)

Removes matching entries from the notification center’s dispatch table.

func removeObserver(Any)

Removes all entries specifying an observer from the notification center’s dispatch table.

