

- XCTest
- XCTWaiter
-  wait(for:timeout:enforceOrder:) 

Type Method

# wait(for:timeout:enforceOrder:)

Creates a waiter that waits on a group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

``` source
class func wait(
    for expectations: [XCTestExpectation],
    timeout seconds: TimeInterval,
    enforceOrder enforceOrderOfFulfillment: Bool
) -> XCTWaiter.Result
```

## Parameters 

`expectations`  

An array of expectations the test must satisfy.

`seconds`  

The time, in seconds, the test allows for the fulfillment of the expectations. The default timeout allows the test to run until it reaches its execution time allowance.

`enforceOrderOfFulfillment`  

If true, the test must satisfy the expectations in the order they appear in the array.

## Return Value

A value describing the outcome of waiting for `expectations`.

## Discussion

Expectations can appear in the `expectations` array only once. The test discards the waiter when the wait completes.

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

class func wait(for: [XCTestExpectation], timeout: TimeInterval) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations for up to the specified timeout.

enum Result

Result states returned by a waiter when it completes, times out, fails, or is interrupted.

