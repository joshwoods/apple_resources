

- XCTest
- XCTestCase
-  fulfillment(of:timeout:enforceOrder:) 

Instance Method

# fulfillment(of:timeout:enforceOrder:)

Waits on a group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
@nonobjc
func fulfillment(
    of expectations: [XCTestExpectation],
    timeout seconds: TimeInterval = .infinity,
    enforceOrder enforceOrderOfFulfillment: Bool = false
) async
```

## Parameters 

`expectations`  

An array of expectations the test must satisfy.

`seconds`  

The time, in seconds, the test allows for the fulfillment of the expectations. The default timeout allows the test to run until it reaches its execution time allowance.

`enforceOrderOfFulfillment`  

If true, the test must satisfy the expectations in the order they appear in the array.

## Discussion

Use this concurrency-safe alternative to wait(for:timeout:enforceOrder:) in your Swift code. Expectations can only appear in the array once. The method can return before the timeout if the test fulfills all the expectations you provide.

Note

If you don’t specify a timeout when calling this function, enable test timeouts to prevent unfulfilled expectation from hanging the test.

## See Also

### Waiting for Expectations

func wait(for: [XCTestExpectation])

Waits on a group of expectations.

func wait(for: [XCTestExpectation], enforceOrder: Bool)

Waits on a group of expectations optionally enforcing their order of fulfillment.

func wait(for: [XCTestExpectation], timeout: TimeInterval)

Waits for the test to fulfill a set of expectations within a specified time.

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

