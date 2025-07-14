

- XCTest
- XCTWaiter
-  delegate 

Instance Property

# delegate

The delegate to which expectation fulfillment events will be reported.

``` source
weak var delegate: (any XCTWaiterDelegate)? { get set }
```

## See Also

### Responding to Expectation Fulfilment

protocol XCTWaiterDelegate

Defines methods that are called when XCTWaiter expectations are fulfilled correctly or incorrectly.

var fulfilledExpectations: [XCTestExpectation]

An array of expectations that were fulfilled, in order, up until the waiter stopped waiting.

