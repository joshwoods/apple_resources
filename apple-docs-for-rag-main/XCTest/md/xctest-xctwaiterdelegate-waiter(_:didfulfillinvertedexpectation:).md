

- XCTest
- XCTWaiterDelegate
-  waiter(\_:didFulfillInvertedExpectation:) 

Instance Method

# waiter(\_:didFulfillInvertedExpectation:)

Invoked when an expectation whose `isInverted` property is set to `true` is fulfilled.

``` source
optional func waiter(
    _ waiter: XCTWaiter,
    didFulfillInvertedExpectation expectation: XCTestExpectation
)
```

## Discussion

If the delegate is an XCTestCase instance, this will be reported as a test failure.

