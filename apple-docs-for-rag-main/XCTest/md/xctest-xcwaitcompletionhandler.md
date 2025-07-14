

- XCTest
-  XCWaitCompletionHandler 

Type Alias

# XCWaitCompletionHandler

A block the test runner calls when the test fulfills a waiter’s expectations, or when it times out.

``` source
typealias XCWaitCompletionHandler = ((any Error)?) -> Void
```

## Parameters 

`error`  

The error the waiter object encountered while waiting, which can be a timeout or a failure. See XCTestError.Code for a list of possible errors.

## Discussion

Pass a block with this signature to waitForExpectations(timeout:handler:). Your block should handle any errors the waiter object encounters, including a timeout, and should perform assertions when the test fulfills the expectation for the waiter object.

## See Also

### Waiting for Expectations

func fulfillment(of: [XCTestExpectation], timeout: TimeInterval, enforceOrder: Bool) async

Waits on a group of expectations for up to the specified timeout, optionally enforcing their order of fulfillment.

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

struct XCTestError

A type of error that can occur while the test waits to fulfill expectations.

enum Code

Error codes for errors that can occur while the test is waiting to fulfill expectations.

let XCTestErrorDomain: String

The error domain for errors that can occur while the test is waiting to fulfill expectations.

