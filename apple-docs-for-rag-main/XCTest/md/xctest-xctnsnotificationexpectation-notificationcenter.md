

- XCTest
- XCTNSNotificationExpectation
-  notificationCenter 

Instance Property

# notificationCenter

The notification center from which the notification must be posted.

``` source
var notificationCenter: NotificationCenter { get }
```

## See Also

### Expectation Properties

var notificationName: NSNotification.Name

The name of the notification that the expectation is waiting for.

var observedObject: Any?

The object by which the notification must be posted, or nil if the notification can be posted by any object.

