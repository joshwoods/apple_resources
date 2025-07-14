

- XCTest
-  XCTWaiter 

Class

# XCTWaiter

Waits for the fulfillment of a group of expectations.

``` source
class XCTWaiter
```

## Overview

You can use waiters with or without a delegate to respond to events such as completion, timeout, or invalid expectation fulfillment. XCTestCase automatically conforms to the XCTWaiterDelegate protocol and automatically reports timeouts and other unexpected events as test failures.

You can use waiters without a delegate or any association with a test case instance. This allows test support libraries to provide convenience methods for waiting without having to pass test cases through those APIs.

## Topics

### Creating a Waiter

init(delegate: (any XCTWaiterDelegate)?)

Creates a new waiter with the specified delegate.

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

enum Result

Result states returned by a waiter when it completes, times out, fails, or is interrupted.

### Responding to Expectation Fulfilment

var delegate: (any XCTWaiterDelegate)?

The delegate to which expectation fulfillment events will be reported.

protocol XCTWaiterDelegate

Defines methods that are called when XCTWaiter expectations are fulfilled correctly or incorrectly.

var fulfilledExpectations: [XCTestExpectation]

An array of expectations that were fulfilled, in order, up until the waiter stopped waiting.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

