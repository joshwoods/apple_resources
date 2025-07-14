

- XCTest
- XCTDarwinNotificationExpectation
-  handler 

Instance Property

# handler

An optional handler that performs custom evaluation of matching notifications.

``` source
var handler: XCTDarwinNotificationExpectation.Handler? { get set }
```

## Discussion

If provided, the custom handler will be queried each time a matching notification is received to determine whether the expectation should be fulfilled. This allows the handler to check Darwin state variables or perform other logic beyond simply verifying that the notification has been received.

## See Also

### Custom Notification Evaluation

typealias Handler

A custom handler to be called when a matching notification is received.

