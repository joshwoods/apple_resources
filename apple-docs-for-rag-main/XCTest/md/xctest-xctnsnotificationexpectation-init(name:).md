

- XCTest
- XCTNSNotificationExpectation
-  init(name:) 

Initializer

# init(name:)

Creates an expectation that is fulfilled when an `NSNotification` is posted from the default notification center by any object.

``` source
convenience init(name notificationName: NSNotification.Name)
```

## Parameters 

`notificationName`  

The notification name to watch for.

## See Also

### Creating NSNotification Expectations

convenience init(name: NSNotification.Name, object: Any?)

Creates an expectation that is fulfilled when an `NSNotification` is posted from the default notification center by a specific object.

init(name: NSNotification.Name, object: Any?, notificationCenter: NotificationCenter)

Creates an expectation that is fulfilled when an `NSNotification` is posted from a specific notification center, optionally by a specific object.

