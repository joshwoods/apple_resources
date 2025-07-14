

- XCTest
- XCTestExpectation
-  isInverted 

Instance Property

# isInverted

Indicates that the expectation is not intended to happen.

``` source
var isInverted: Bool { get set }
```

## Discussion

To check that a situation does *not* occur during testing, create an expectation that is fulfilled when the unexpected situation occurs, and set its isInverted property to true. Your test will fail immediately if the inverted expectation is fulfilled.

