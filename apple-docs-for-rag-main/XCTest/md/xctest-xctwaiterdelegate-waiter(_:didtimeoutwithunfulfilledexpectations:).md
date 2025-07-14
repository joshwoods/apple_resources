

- XCTest
- XCTWaiterDelegate
-  waiter(\_:didTimeoutWithUnfulfilledExpectations:) 

Instance Method

# waiter(\_:didTimeoutWithUnfulfilledExpectations:)

Invoked when not all waited on expectations are fulfilled during the timeout period.

``` source
optional func waiter(
    _ waiter: XCTWaiter,
    didTimeoutWithUnfulfilledExpectations unfulfilledExpectations: [XCTestExpectation]
)
```

## Parameters 

`waiter`  

The XCTWaiter reporting the timeout event.

`unfulfilledExpectations`  

The expectations

## Discussion

If the delegate is an XCTestCase instance, this will be reported as a test failure.

## See Also

### Timeout Events

func nestedWaiter(XCTWaiter, wasInterruptedByTimedOutWaiter: XCTWaiter)

Invoked when the waiter is interrupted prior to its expectations being fulfilled or timing out.

