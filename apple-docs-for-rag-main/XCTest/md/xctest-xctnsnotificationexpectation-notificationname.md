

- XCTest
- XCTNSNotificationExpectation
-  notificationName 

Instance Property

# notificationName

The name of the notification that the expectation is waiting for.

``` source
var notificationName: NSNotification.Name { get }
```

## See Also

### Expectation Properties

var observedObject: Any?

The object by which the notification must be posted, or nil if the notification can be posted by any object.

var notificationCenter: NotificationCenter

The notification center from which the notification must be posted.

