

- XCTest
- XCTNSNotificationExpectation
-  init(name:object:) 

Initializer

# init(name:object:)

Creates an expectation that is fulfilled when an `NSNotification` is posted from the default notification center by a specific object.

``` source
convenience init(
    name notificationName: NSNotification.Name,
    object: Any?
)
```

## Parameters 

`notificationName`  

The notification name to watch for.

`object`  

The object by which the notification must be posted.

## See Also

### Creating NSNotification Expectations

convenience init(name: NSNotification.Name)

Creates an expectation that is fulfilled when an `NSNotification` is posted from the default notification center by any object.

init(name: NSNotification.Name, object: Any?, notificationCenter: NotificationCenter)

Creates an expectation that is fulfilled when an `NSNotification` is posted from a specific notification center, optionally by a specific object.

