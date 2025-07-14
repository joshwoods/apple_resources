

- XCTest
- XCTNSNotificationExpectation
-  observedObject 

Instance Property

# observedObject

The object by which the notification must be posted, or nil if the notification can be posted by any object.

``` source
var observedObject: Any? { get }
```

## See Also

### Expectation Properties

var notificationName: NSNotification.Name

The name of the notification that the expectation is waiting for.

var notificationCenter: NotificationCenter

The notification center from which the notification must be posted.

