

- XCTest
- XCTNSNotificationExpectation
-  XCTNSNotificationExpectation.Handler 

Type Alias

# XCTNSNotificationExpectation.Handler

A custom handler to be called when a matching notification is received.

``` source
typealias Handler = (Notification) -> Bool
```

## Parameters 

`notification`  

The notification object.

## Return Value

Your custom handler should return true if the expectation is considered fulfilled after the notification is received, otherwise false.

## See Also

### Custom Notification Evaluation

var handler: XCTNSNotificationExpectation.Handler?

An optional handler that performs custom evaluation of matching notifications.

