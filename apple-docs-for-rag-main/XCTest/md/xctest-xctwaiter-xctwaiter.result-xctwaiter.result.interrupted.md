

- XCTest
- XCTWaiter
- XCTWaiter.Result
-  XCTWaiter.Result.interrupted 

Case

# XCTWaiter.Result.interrupted

The waiter was interrupted prior to its expectations being fulfilled or timing out.

``` source
case interrupted
```

## Discussion

This occurs when an “outer” waiter times out, resulting in any waiters nested inside it being interrupted to allow the call stack to quickly unwind.

## See Also

### Result States

case completed

All of the waiter’s expectations were fulfilled successfully.

case timedOut

The waiter timed out before all of its expectations were fulfilled.

case incorrectOrder

The waiter’s expectations were not fulfilled in the required order.

case invertedFulfillment

An inverted expectation was fulfilled.

