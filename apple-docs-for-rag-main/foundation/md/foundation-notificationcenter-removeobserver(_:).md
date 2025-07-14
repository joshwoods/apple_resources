

- Foundation
- NotificationCenter
-  removeObserver(\_:) 

Instance Method

# removeObserver(\_:)

Removes all entries specifying an observer from the notification center’s dispatch table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObserver(_ observer: Any)
```

## Parameters 

`observer`  

The observer to remove from the dispatch table. Specify an observer to remove only entries for this observer.

## Discussion

Removing the observer stops it from receiving notifications.

If you used addObserver(forName:object:queue:using:) to create your observer, you should call this method or removeObserver(_:name:object:) before the system deallocates any object that addObserver(forName:object:queue:using:) specifies.

If your app targets iOS 9.0 and later or macOS 10.11 and later, and you used addObserver(_:selector:name:object:), you do not need to unregister the observer. If you forget or are unable to remove the observer, the system cleans up the next time it would have posted to it.

When removing an observer, remove it with the most specific detail possible. For example, if you used a name and object to register the observer, use removeObserver(_:name:object:) with the name and object.

Important

You shouldn’t use this method to remove all observers from a long-lived object because your code may not be the only code adding observers that involve the object.

The following example illustrates how to unregister `someObserver` for all previously registered notifications. This is safe to do in the dealloc method, but you shouldn’t use it otherwise (use removeObserver(_:name:object:) instead).

- Swift
- Objective-C

```
NotificationCenter.default.removeObserver(someObserver)
```

```
[[NSNotificationCenter defaultCenter] removeObserver:someObserver];
```

## See Also

### Adding and Removing Notification Observers

func addObserver(forName: NSNotification.Name?, object: Any?, queue: OperationQueue?, using: (Notification) -> Void) -> any NSObjectProtocol

Adds an entry to the notification center to receive notifications that passed to the provided block.

func addObserver(Any, selector: Selector, name: NSNotification.Name?, object: Any?)

Adds an entry to the notification center to call the provided selector with the notification.

func removeObserver(Any, name: NSNotification.Name?, object: Any?)

Removes matching entries from the notification center’s dispatch table.

