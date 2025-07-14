

- XCTest
- XCTWaiter
-  XCTWaiter.Result 

Enumeration

# XCTWaiter.Result

Result states returned by a waiter when it completes, times out, fails, or is interrupted.

``` source
enum Result
```

## Topics

### Result States

case completed

All of the waiter’s expectations were fulfilled successfully.

case timedOut

The waiter timed out before all of its expectations were fulfilled.

case incorrectOrder

The waiter’s expectations were not fulfilled in the required order.

case invertedFulfillment

An inverted expectation was fulfilled.

case interrupted

The waiter was interrupted prior to its expectations being fulfilled or timing out.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Waiting for Expectations

func fulfillment(of: [XCTestExpectation], timeout: TimeInterval, enforceOrder: Bool) async -> XCTWaiter.Result

Waits on a group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

func wait(for: [XCTestExpectation]) -> XCTWaiter.Result

Waits on a group of expectations.

func wait(for: [XCTestExpectation], enforceOrder: Bool) -> XCTWaiter.Result

Waits on a group of expectations optionally enforcing their order of fulfillment.

func wait(for: [XCTestExpectation], timeout: TimeInterval) -> XCTWaiter.Result

Waits on a group of expectations for up to the specified timeout.

func wait(for: [XCTestExpectation], timeout: TimeInterval, enforceOrder: Bool) -> XCTWaiter.Result

Waits on a group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

class func fulfillment(of: [XCTestExpectation], timeout: TimeInterval, enforceOrder: Bool) async -> XCTWaiter.Result

Creates a waiter that waits on group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

class func wait(for: [XCTestExpectation]) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations.

class func wait(for: [XCTestExpectation], enforceOrder: Bool) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations optionally enforcing their order of fulfillment.

class func wait(for: [XCTestExpectation], timeout: TimeInterval) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations for up to the specified timeout.

class func wait(for: [XCTestExpectation], timeout: TimeInterval, enforceOrder: Bool) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

