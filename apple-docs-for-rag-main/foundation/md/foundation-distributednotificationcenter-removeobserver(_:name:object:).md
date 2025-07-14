

- Foundation
- DistributedNotificationCenter
-  removeObserver(\_:name:object:) 

Instance Method

# removeObserver(\_:name:object:)

Removes matching entries from the receiver’s dispatch table.

Mac Catalyst 13.0+macOS 10.0+

``` source
func removeObserver(
    _ observer: Any,
    name aName: NSNotification.Name?,
    object anObject: String?
)
```

## Parameters 

`observer`  

Observer to remove from the dispatch table. Specify an observer to remove only entries for this observer. When `nil`, the receiver does not use notification observers as criteria for removal.

`aName`  

Name of the notification to remove from dispatch table. Specify a notification name to remove only entries that specify this notification name. When `nil`, the receiver does not use notification names as criteria for removal.

`anObject`  

Sender to remove from the dispatch table. Specify a notification sender to remove only entries that specify this sender. When `nil`, the receiver does not use notification senders as criteria for removal.

## Discussion

Be sure to invoke this method with `notificationName:nil notificationSender:nil` (or removeObserver(_:)) before deallocating the observer object.

## See Also

### Managing Observers

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: String?)

Adds an entry to the notification center’s dispatch table with an observer, a selector, and an optional notification name and sender.

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: String?, suspensionBehavior: DistributedNotificationCenter.SuspensionBehavior)

Adds an entry to the receiver’s dispatch table with a specific observer and suspended-notifications behavior, and optional notification name and sender.

