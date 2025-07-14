

- XCTest
- XCTestCase
-  wait(for:timeout:) 

Instance Method

# wait(for:timeout:)

Waits for the test to fulfill a set of expectations within a specified time.

``` source
func wait(
    for expectations: [XCTestExpectation],
    timeout seconds: TimeInterval
)
```

## Parameters 

`expectations`  

An array of expectations the test must satisfy.

`seconds`  

The time, in seconds, the test allows for the fulfillment of the expectations. The default timeout allows the test to run until it reaches its execution time allowance.

## Discussion

Note

Use fulfillment(of:timeout:enforceOrder:) in Swift code requiring concurrency.

In Objective-C code, you might use an expectation to wait on a call to an interface that uses a completion handler to return a result. From Swift code, consider calling `withCheckedContinuation(function:_:)` to use Concurrency instead of an expectation to wait on the result of a completion handler.

## See Also

### Waiting for Expectations

func fulfillment(of: [XCTestExpectation], timeout: TimeInterval, enforceOrder: Bool) async

Waits on a group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

func wait(for: [XCTestExpectation])

Waits on a group of expectations.

func wait(for: [XCTestExpectation], enforceOrder: Bool)

Waits on a group of expectations optionally enforcing their order of fulfillment.

func wait(for: [XCTestExpectation], timeout: TimeInterval, enforceOrder: Bool)

Waits for the test to satisfy an array of expectations and specifies whether they must occur in the array’s order.

func waitForExpectations(timeout: TimeInterval, handler: (((any Error)?) -> Void)?)

Waits until the test fulfills all expectations or until it times out.

typealias XCWaitCompletionHandler

A block the test runner calls when the test fulfills a waiter’s expectations, or when it times out.

struct XCTestError

A type of error that can occur while the test waits to fulfill expectations.

enum Code

Error codes for errors that can occur while the test is waiting to fulfill expectations.

let XCTestErrorDomain: String

The error domain for errors that can occur while the test is waiting to fulfill expectations.

