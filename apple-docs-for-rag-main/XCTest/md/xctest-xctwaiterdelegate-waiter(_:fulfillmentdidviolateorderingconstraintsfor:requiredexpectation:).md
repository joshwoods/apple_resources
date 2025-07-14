

- XCTest
- XCTWaiterDelegate
-  waiter(\_:fulfillmentDidViolateOrderingConstraintsFor:requiredExpectation:) 

Instance Method

# waiter(\_:fulfillmentDidViolateOrderingConstraintsFor:requiredExpectation:)

Invoked when a waiter is enforcing fulfillment order and an expectation is fulfilled in the wrong order.

``` source
optional func waiter(
    _ waiter: XCTWaiter,
    fulfillmentDidViolateOrderingConstraintsFor expectation: XCTestExpectation,
    requiredExpectation: XCTestExpectation
)
```

## Discussion

If the delegate is an XCTestCase instance, this will be reported as a test failure.

