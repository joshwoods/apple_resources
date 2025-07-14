

- XCTest
-  XCTestExpectation 

Class

# XCTestExpectation

An expected outcome in an asynchronous test.

``` source
class XCTestExpectation
```

## Topics

### Creating Expectations

init(description: String)

Creates a new XCTestExpectation with the provided description.

var expectationDescription: String

A human readable string used to describe the expectation in log output and test reports.

### Fulfilling Expectations

func fulfill()

Marks the expectation as having been met.

### Fulfillment Count

var expectedFulfillmentCount: Int

The number of times fulfill() must be called before the expectation is completely fulfilled.

var assertForOverFulfill: Bool

Indicates that an assertion should be triggered during testing if the expectation is over-fulfilled.

### Unintended Expectations

var isInverted: Bool

Indicates that the expectation is not intended to happen.

## Relationships

### Inherits From

- NSObject

### Inherited By

- XCTDarwinNotificationExpectation
- XCTKVOExpectation
- XCTKeyPathExpectation
- XCTNSNotificationExpectation
- XCTNSPredicateExpectation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

