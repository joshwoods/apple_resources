

- XCTest
-  XCTNSNotificationExpectation 

Class

# XCTNSNotificationExpectation

An expectation that is fulfilled when an expected `NSNotification` is received.

``` source
class XCTNSNotificationExpectation
```

## Topics

### Creating NSNotification Expectations

convenience init(name: NSNotification.Name)

Creates an expectation that is fulfilled when an `NSNotification` is posted from the default notification center by any object.

convenience init(name: NSNotification.Name, object: Any?)

Creates an expectation that is fulfilled when an `NSNotification` is posted from the default notification center by a specific object.

init(name: NSNotification.Name, object: Any?, notificationCenter: NotificationCenter)

Creates an expectation that is fulfilled when an `NSNotification` is posted from a specific notification center, optionally by a specific object.

### Expectation Properties

var notificationName: NSNotification.Name

The name of the notification that the expectation is waiting for.

var observedObject: Any?

The object by which the notification must be posted, or nil if the notification can be posted by any object.

var notificationCenter: NotificationCenter

The notification center from which the notification must be posted.

### Custom Notification Evaluation

var handler: XCTNSNotificationExpectation.Handler?

An optional handler that performs custom evaluation of matching notifications.

typealias Handler

A custom handler to be called when a matching notification is received.

## Relationships

### Inherits From

- XCTestExpectation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Notification-Based Expectations

class XCTDarwinNotificationExpectation

An expectation that is fulfilled when an expected Darwin notification is received.

