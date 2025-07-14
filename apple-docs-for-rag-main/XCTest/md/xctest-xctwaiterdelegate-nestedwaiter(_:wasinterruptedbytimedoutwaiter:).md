

- XCTest
- XCTWaiterDelegate
-  nestedWaiter(\_:wasInterruptedByTimedOutWaiter:) 

Instance Method

# nestedWaiter(\_:wasInterruptedByTimedOutWaiter:)

Invoked when the waiter is interrupted prior to its expectations being fulfilled or timing out.

``` source
optional func nestedWaiter(
    _ waiter: XCTWaiter,
    wasInterruptedByTimedOutWaiter outerWaiter: XCTWaiter
)
```

## Discussion

This occurs when an “outer” waiter times out, resulting in any waiters nested inside it being interrupted to allow the call stack to quickly unwind.

## See Also

### Timeout Events

func waiter(XCTWaiter, didTimeoutWithUnfulfilledExpectations: [XCTestExpectation])

Invoked when not all waited on expectations are fulfilled during the timeout period.

