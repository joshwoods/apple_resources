

- XCTest
- XCTWaiter
-  wait(for:timeout:) 

Type Method

# wait(for:timeout:)

Creates a waiter that waits on a group of expectations for up to the specified timeout.

``` source
class func wait(
    for expectations: [XCTestExpectation],
    timeout seconds: TimeInterval
) -> XCTWaiter.Result
```

## Parameters 

`expectations`  

An array of expectations the test must satisfy.

`seconds`  

The time, in seconds, the test allows for the fulfillment of the expectations. The default timeout allows the test to run until it reaches its execution time allowance.

## Return Value

A value describing the outcome of waiting for `expectations`.

## Discussion

Expectations can only appear in the array once. The test discards the waiter when the wait completes.

In Objective-C code, you might use an expectation to wait on a call to an interface that uses a completion handler to return a result. From Swift code, consider calling `withCheckedContinuation(function:_:)` to use Concurrency instead of an expectation to wait on the result of a completion handler.

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

class func wait(for: [XCTestExpectation], timeout: TimeInterval, enforceOrder: Bool) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

enum Result

Result states returned by a waiter when it completes, times out, fails, or is interrupted.

