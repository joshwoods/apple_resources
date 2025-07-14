

- XCTest
-  XCTDarwinNotificationExpectation 

Class

# XCTDarwinNotificationExpectation

An expectation that is fulfilled when an expected Darwin notification is received.

``` source
class XCTDarwinNotificationExpectation
```

## Overview

If a custom handler value is not provided, the expectation will be fulfilled as soon as a matching Darwin notification is received from any process.

## Topics

### Creating Darwin Notification Expectations

init(notificationName: String)

Creates an expectation that waits for a Darwin notification with the specified name to be posted.

### Expectation Properties

var notificationName: String

The name of the notification that the expectation is waiting for.

### Custom Notification Evaluation

var handler: XCTDarwinNotificationExpectation.Handler?

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

class XCTNSNotificationExpectation

An expectation that is fulfilled when an expected `NSNotification` is received.

