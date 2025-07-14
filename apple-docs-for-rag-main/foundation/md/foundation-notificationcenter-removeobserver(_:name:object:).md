

- Foundation
- NotificationCenter
-  removeObserver(\_:name:object:) 

Instance Method

# removeObserver(\_:name:object:)

Removes matching entries from the notification center’s dispatch table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObserver(
    _ observer: Any,
    name aName: NSNotification.Name?,
    object anObject: Any?
)
```

## Parameters 

`observer`  

The observer to remove from the dispatch table. Specify an observer to remove only entries for this observer.

`aName`  

The name of the notification to remove from the dispatch table. Specify a notification name to remove only entries with this notification name. When `nil`, the receiver does not use notification names as criteria for removal.

`anObject`  

The sender to remove from the dispatch table. Specify a notification sender to remove only entries with this sender. When `nil`, the receiver does not use a sender as criteria for removal.

## Discussion

Removing the observer stops it from receiving notifications.

If you used addObserver(forName:object:queue:using:) to create your observer, you should call this method or removeObserver(_:) before the system deallocates any object that addObserver(forName:object:queue:using:) specifies.

If your app targets iOS 9.0 and later or macOS 10.11 and later, and you used addObserver(_:selector:name:object:) to create your observer, you do not need to unregister the observer. If you forget or are unable to remove the observer, the system cleans up the next time it would have posted to it.

When unregistering an observer, use the most specific detail possible. For example, if you used a name and object to register the observer, use removeObserver(_:name:object:) with the name and object.

## See Also

### Adding and Removing Notification Observers

func addObserver(forName: NSNotification.Name?, object: Any?, queue: OperationQueue?, using: (Notification) -> Void) -> any NSObjectProtocol

Adds an entry to the notification center to receive notifications that passed to the provided block.

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: Any?)

Adds an entry to the notification center to call the provided selector with the notification.

func removeObserver(Any)

Removes all entries specifying an observer from the notification center’s dispatch table.

