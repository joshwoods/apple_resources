

- XCTest
- XCTDarwinNotificationExpectation
-  XCTDarwinNotificationExpectation.Handler 

Type Alias

# XCTDarwinNotificationExpectation.Handler

A custom handler to be called when a matching notification is received.

``` source
typealias Handler = () -> Bool
```

## Return Value

Your custom handler should return true if the expectation is considered fulfilled after the notification is received, otherwise false.

## See Also

### Custom Notification Evaluation

var handler: XCTDarwinNotificationExpectation.Handler?

An optional handler that performs custom evaluation of matching notifications.

