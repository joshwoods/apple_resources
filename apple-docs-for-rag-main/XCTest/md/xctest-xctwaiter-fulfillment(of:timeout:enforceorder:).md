

- XCTest
- XCTWaiter
-  fulfillment(of:timeout:enforceOrder:) 

Type Method

# fulfillment(of:timeout:enforceOrder:)

Creates a waiter that waits on group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
@nonobjc
class func fulfillment(
    of expectations: [XCTestExpectation],
    timeout seconds: TimeInterval = .infinity,
    enforceOrder enforceOrderOfFulfillment: Bool = false
) async -> XCTWaiter.Result
```

## Parameters 

`expectations`  

An array of expectations the test must satisfy.

`seconds`  

The time, in seconds, the test allows for the fulfillment of the expectations.

`enforceOrderOfFulfillment`  

If true, the test must satisfy the expectations in the order they appear in the array.

## Return Value

A value describing the outcome of waiting for `expectations`.

## Discussion

Use this Concurrency safe alternative to wait(for:timeout:enforceOrder:) in your Swift code. A call to wait(for:timeout:enforceOrder:) runs synchronously and blocks the calling thread, which can cause deadlocks or priority inversion.

Expectations can only appear in the array once. The call may return before the timeout if the test fulfills all the expectations you provide.

Note

If you don’t specify a timeout when calling this function, enable test timeouts to prevent unfulfilled expectation from hanging the test.

The test discards the waiter after the wait completes.

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

class func wait(for: [XCTestExpectation]) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations.

class func wait(for: [XCTestExpectation], enforceOrder: Bool) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations optionally enforcing their order of fulfillment.

class func wait(for: [XCTestExpectation], timeout: TimeInterval) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations for up to the specified timeout.

class func wait(for: [XCTestExpectation], timeout: TimeInterval, enforceOrder: Bool) -> XCTWaiter.Result

Creates a waiter that waits on a group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

enum Result

Result states returned by a waiter when it completes, times out, fails, or is interrupted.

