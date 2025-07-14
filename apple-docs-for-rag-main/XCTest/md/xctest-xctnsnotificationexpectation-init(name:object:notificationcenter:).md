

- XCTest
- XCTNSNotificationExpectation
-  init(name:object:notificationCenter:) 

Initializer

# init(name:object:notificationCenter:)

Creates an expectation that is fulfilled when an `NSNotification` is posted from a specific notification center, optionally by a specific object.

``` source
init(
    name notificationName: NSNotification.Name,
    object: Any?,
    notificationCenter: NotificationCenter
)
```

## Parameters 

`notificationName`  

The notification name to watch for.

`object`  

The object by which the notification must be posted, or nil if the notification can be posted by any object.

`notificationCenter`  

The NotificationCenter from which the notification must be posted.

## See Also

### Creating NSNotification Expectations

convenience init(name: NSNotification.Name)

Creates an expectation that is fulfilled when an `NSNotification` is posted from the default notification center by any object.

convenience init(name: NSNotification.Name, object: Any?)

Creates an expectation that is fulfilled when an `NSNotification` is posted from the default notification center by a specific object.

