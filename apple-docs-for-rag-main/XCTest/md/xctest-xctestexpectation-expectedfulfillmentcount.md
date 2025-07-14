

- XCTest
- XCTestExpectation
-  expectedFulfillmentCount 

Instance Property

# expectedFulfillmentCount

The number of times fulfill() must be called before the expectation is completely fulfilled.

``` source
var expectedFulfillmentCount: Int { get set }
```

## Discussion

The value of expectedFulfillmentCount must be greater than 0. By default, expectations have an expectedFulfillmentCount of 1.

Note

The value of expectedFulfillmentCount is ignored when isInverted is true.

## See Also

### Fulfillment Count

var assertForOverFulfill: Bool

Indicates that an assertion should be triggered during testing if the expectation is over-fulfilled.

