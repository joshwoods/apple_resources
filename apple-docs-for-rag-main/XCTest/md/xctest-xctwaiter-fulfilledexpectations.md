

- XCTest
- XCTWaiter
-  fulfilledExpectations 

Instance Property

# fulfilledExpectations

An array of expectations that were fulfilled, in order, up until the waiter stopped waiting.

``` source
var fulfilledExpectations: [XCTestExpectation] { get }
```

## Discussion

The array will be empty until the waiter has started waiting, even if expectations have already been fulfilled. Expectations fulfilled after the waiter stops waiting will not be in the array.

## See Also

### Responding to Expectation Fulfilment

var delegate: (any XCTWaiterDelegate)?

The delegate to which expectation fulfillment events will be reported.

protocol XCTWaiterDelegate

Defines methods that are called when XCTWaiter expectations are fulfilled correctly or incorrectly.

