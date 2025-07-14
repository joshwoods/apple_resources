

- XCTest
- XCTestExpectation
-  assertForOverFulfill 

Instance Property

# assertForOverFulfill

Indicates that an assertion should be triggered during testing if the expectation is over-fulfilled.

``` source
var assertForOverFulfill: Bool { get set }
```

## Discussion

When true, a call to fulfill() made after the expectation has already been fulfilled (exceeding expectedFulfillmentCount) will trigger an assertion. When false, a call to fulfill() after the expectation has already been fulfilled will have no effect.

The assertForOverFulfill property is set to false by default for expectations created directly from initializers on XCTestExpectation and its subclasses.

The assertForOverFulfill property is set to true by default for expectations created with the following XCTestCase convenience methods:

- expectation(description:)

- expectation(for:evaluatedWith:handler:)

- expectation(forNotification:object:handler:)

- keyValueObservingExpectation(for:keyPath:expectedValue:)

- keyValueObservingExpectation(for:keyPath:handler:)

## See Also

### Fulfillment Count

var expectedFulfillmentCount: Int

The number of times fulfill() must be called before the expectation is completely fulfilled.

